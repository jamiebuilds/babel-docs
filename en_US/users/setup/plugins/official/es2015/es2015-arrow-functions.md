# ES2015 Arrow Functions

Compile ES2015 arrow functions to ES5

## Example

**Input**

```js
arr.map(x => x * x);
```

**Output**

```js
arr.map(function (x) {
  return x * x;
});
```

> Note that the output may not be exactly what is above. Babel's implementation
> may have changed since this document was last updated, or the output may have
> been cleaned up for clarity.

## Setup

### Installation

```sh
$ npm install --save-dev babel-plugin-transform-es2015-arrow-functions
```

### Usage

#### Via `.babelrc` (recommended)

**`.babelrc`**

```json
{
  "plugins": ["transform-es2015-arrow-functions"]
}
```

#### Via CLI

```sh
babel script.js --plugin transform-es2015-arrow-functions
```

#### Via Node API

```js
require("babel-core").transform("code", {
  plugins: ["transform-es2015-arrow-functions"]
});
```
