# ES2015 function.name

Apply ES2015 function.name semantics to all functions

## Example

**Input**

```js
var method = function() {
  // ...
};
```

**Output**

```js
var method = function method() {
  // ...
};
```

> Note that the output may not be exactly what is above. Babel's implementation
> may have changed since this document was last updated, or the output may have
> been cleaned up for clarity.

## Setup

### Installation

```sh
$ npm install --save-dev babel-plugin-transform-es2015-function-name
```

### Usage

#### Via `.babelrc` (recommended)

**`.babelrc`**

```json
{
  "plugins": ["transform-es2015-function-name"]
}
```

#### Via CLI

```sh
babel script.js --plugin transform-es2015-function-name
```

#### Via Node API

```js
require("babel-core").transform("code", {
  plugins: ["transform-es2015-function-name"]
});
```
