# Building Nodes

When writing transformations you'll often want to build up some nodes to insert
into the AST. As mentioned previously, you can do this using the
[builder](#builder) methods in the [`babel-types`](#babel-types) package.

The method name for a builder is simply the name of the node type you want to
build except with the first letter lowercased. For example if you wanted to
build a `MemberExpression` you would use `t.memberExpression(...)`.

The arguments of these builders are decided by the node definition. There's some
work that's being done to generate easy-to-read documentation on the
definitions, but for now they can all be found
[here](https://github.com/babel/babel/tree/master/packages/babel-types/src/definitions).

A node definition looks like the following:

```js
defineType("MemberExpression", {
  builder: ["object", "property", "computed"],
  visitor: ["object", "property"],
  aliases: ["Expression", "LVal"],
  fields: {
    object: {
      validate: assertNodeType("Expression")
    },
    property: {
      validate(node, key, val) {
        let expectedType = node.computed ? "Expression" : "Identifier";
        assertNodeType(expectedType)(node, key, val);
      }
    },
    computed: {
      default: false
    }
  }
});
```

Here you can see all the information about this particular node type, including
how to build it, traverse it, and validate it.

By looking at the `builder` property, you can see the 3 arguments that will be
needed to call the builder method (`t.memberExpression`).

```js
builder: ["object", "property", "computed"],
```

> Note that sometimes there are more properties that you can customize on the
> node than the `builder` array contains. This is to keep the builder from
> having too many arguments. In these cases you need to set the properties
> manually. An example of this is
> [`ClassMethod`](https://github.com/babel/babel/blob/bbd14f88c4eea88fa584dd877759dd6b900bf35e/packages/babel-types/src/definitions/es2015.js#L238-L276).

You can see the validation for the builder arguments with the `fields` object.

```js
fields: {
  object: {
    validate: assertNodeType("Expression")
  },
  property: {
    validate(node, key, val) {
      let expectedType = node.computed ? "Expression" : "Identifier";
      assertNodeType(expectedType)(node, key, val);
    }
  },
  computed: {
    default: false
  }
}
```

You can see that `object` needs to be an `Expression`, `property` either needs
to be an `Expression` or an `Identifier` depending on if the member expression
is `computed` or not and `computed` is simply a boolean that defaults to
`false`.

So we can construct a `MemberExpression` by doing the following:

```js
t.memberExpression(
  t.identifier('object'),
  t.identifier('property')
  // `computed` is optional
);
```

Which will result in:

```js
object.property
```

However, we said that `object` needed to be an `Expression` so why is
`Identifier` valid?

Well if we look at the definition of `Identifier` we can see that it has an
`aliases` property which states that it is also an expression.

```js
aliases: ["Expression", "LVal"],
```

So since `MemberExpression` is a type of `Expression`, we could set it as the
`object` of another `MemberExpression`:

```js
t.memberExpression(
  t.memberExpression(
    t.identifier('member'),
    t.identifier('expression')
  ),
  t.identifier('property')
)
```

Which will result in:

```js
member.expression.property
```

It's very unlikely that you will ever memorize the builder method signatures for
every node type. So you should take some time and understand how they are
generated from the node definitions.

You can find all of the actual
[definitions here](https://github.com/babel/babel/tree/master/packages/babel-types/src/definitions)
and you can see them
[documented here](https://github.com/babel/babel/blob/master/doc/ast/spec.md)
