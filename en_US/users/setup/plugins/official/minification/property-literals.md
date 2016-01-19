# Property Literals

Turn valid property key literals to plain identifiers

## Example

**Input**

```js
var obj = {
  "foo": "isValid",
  var: "isKeyword",
  "const": "isKeyword"
};
```

**Output**

```js
var obj = {
  foo: "isValid",
  "var": "isKeyword",
  "const": "isKeyword"
};
```

> Note that the output may not be exactly what is above. Babel's implementation
> may have changed since this document was last updated, or the output may have
> been cleaned up for clarity.

## Setup

### Installation

```sh
$ npm install --save-dev babel-plugin-transform-property-literals
```

### Usage

#### Via `.babelrc` (recommended)

**`.babelrc`**

```json
{
  "plugins": ["transform-property-literals"]
}
```

#### Via CLI

```sh
babel script.js --plugin transform-property-literals
```

#### Via Node API

```js
require("babel-core").transform("code", {
  plugins: ["transform-property-literals"]
});
```
