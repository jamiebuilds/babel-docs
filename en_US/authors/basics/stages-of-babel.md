## Stages of Babel

The three primary stages of Babel are **parse**, **transform**, **generate**.

### Parse

The **parse** stage, takes code and outputs an AST. There are two phases of
parsing in Babel:
[**Lexical Analysis**](https://en.wikipedia.org/wiki/Lexical_analysis) and
[**Syntactic Analysis**](https://en.wikipedia.org/wiki/Parsing).

#### Lexical Analysis

Lexical Analysis will take a string of code and turn it into a stream of
**tokens**.

You can think of tokens as a flat array of language syntax pieces.

```js
n * n;
```

```js
[
  { type: { ... }, value: "n", start: 0, end: 1, loc: { ... } },
  { type: { ... }, value: "*", start: 2, end: 3, loc: { ... } },
  { type: { ... }, value: "n", start: 4, end: 5, loc: { ... } },
  ...
]
```

Each of the `type`s here have a set of properties describing the token:

```js
{
  type: {
    label: 'name',
    keyword: undefined,
    beforeExpr: false,
    startsExpr: true,
    rightAssociative: false,
    isLoop: false,
    isAssign: false,
    prefix: false,
    postfix: false,
    binop: null,
    updateContext: null
  },
  ...
}
```

Like AST nodes they also have a `start`, `end`, and `loc`.

#### Syntactic Analysis

Syntactic Analysis will take a stream of tokens and turn it into an AST
representation. Using the information in the tokens, this phase will reformat
them as an AST which represents the structure of the code in a way that makes it
easier to work with.

### Transform

The [transform](https://en.wikipedia.org/wiki/Program_transformation) stage
takes an AST and traverses through it, adding, updating, and removing nodes as
it goes along. This is by far the most complex part of Babel or any compiler.
This is where plugins operate and so it will be the subject of most of this
handbook. So we won't dive too deep right now.

### Generate

The [code generation](https://en.wikipedia.org/wiki/Code_generation_(compiler))
stage takes the final AST and turns in back into a string of code, also creating
[source maps](http://www.html5rocks.com/en/tutorials/developertools/sourcemaps/).

Code generation is pretty simple: you traverse through the AST depth-first,
building a string that represents the transformed code.
