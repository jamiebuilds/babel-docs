Each of these steps involve creating or working with an
[Abstract Syntax Tree](https://en.wikipedia.org/wiki/Abstract_syntax_tree) or
AST.

> Babel uses an AST modified from [ESTree](https://github.com/estree/estree),
> with the core spec located
> [here](https://github.com/babel/babel/blob/master/doc/ast/spec.md).

```js
function square(n) {
  return n * n;
}
```

> Check out [AST Explorer](http://astexplorer.net/) to get a better sense of the
> AST nodes. [Here](http://astexplorer.net/#/Z1exs6BWMq) is a link to it with
> the example code above pasted in.

This same program can be represented as a list like this:

```md
- FunctionDeclaration:
  - id:
    - Identifier:
      - name: square
  - params [1]
    - Identifier
      - name: n
  - body:
    - BlockStatement
      - body [1]
        - ReturnStatement
          - argument
            - BinaryExpression
              - operator: *
              - left
                - Identifier
                  - name: n
              - right
                - Identifier
                  - name: n
```

Or as a JavaScript Object like this:

```js
{
  type: "FunctionDeclaration",
  id: {
    type: "Identifier",
    name: "square"
  },
  params: [{
    type: "Identifier",
    name: "n"
  }],
  body: {
    type: "BlockStatement",
    body: [{
      type: "ReturnStatement",
      argument: {
        type: "BinaryExpression",
        operator: "*",
        left: {
          type: "Identifier",
          name: "n"
        },
        right: {
          type: "Identifier",
          name: "n"
        }
      }
    }]
  }
}
```

You'll notice that each level of the AST has a similar structure:

```js
{
  type: "FunctionDeclaration",
  id: {...},
  params: [...],
  body: {...}
}
```

```js
{
  type: "Identifier",
  name: ...
}
```

```js
{
  type: "BinaryExpression",
  operator: ...,
  left: {...},
  right: {...}
}
```

> Note: Some properties have been removed for simplicity.

Each of these are known as a **Node**. An AST can be made up of a single Node,
or hundreds if not thousands of Nodes. Together they are able to describe the
syntax of a program that can be used for static analysis.

Every Node has this interface:

```typescript
interface Node {
  type: string;
}
```

The `type` field is a string representing the type of Node the object is (ie.
`"FunctionDeclaration"`, `"Identifier"`, or `"BinaryExpression"`). Each type of
Node defines an additional set of properties that describe that particular node
type.

There are additional properties on every Node that Babel generates which
describe the position of the Node in the original source code.

```js
{
  type: ...,
  start: 0,
  end: 38,
  loc: {
    start: {
      line: 1,
      column: 0
    },
    end: {
      line: 3,
      column: 1
    }
  },
  ...
}
```

These properties `start`, `end`, `loc`, appear in every single Node.
