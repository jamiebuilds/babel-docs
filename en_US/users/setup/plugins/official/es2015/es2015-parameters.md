# ES2015 Parameters

Compile ES2015 default and rest parameters to ES5

## Example

**Input**

```js
function method(param = "default") {
  // ...
}
function method2(...rest) {
  // ...
}
```

**Output**

```js
function method() {
  var param = arguments.length <= 0 || arguments[0] === undefined ? "default" : arguments[0];
  // ...
}
function method2(...rest) {
  for (var _len = arguments.length, rest = Array(_len), _key = 0; _key < _len; _key++) {
    b[_key] = arguments[_key];
  }
  // ...
}
```

> Note that the output may not be exactly what is above. Babel's implementation
> may have changed since this document was last updated, or the output may have
> been cleaned up for clarity.

## Setup

### Installation

```sh
$ npm install --save-dev babel-plugin-transform-es2015-parameters
```

### Usage

#### Via `.babelrc` (recommended)

**`.babelrc`**

```json
{
  "plugins": ["transform-es2015-parameters"]
}
```

#### Via CLI

```sh
babel script.js --plugin transform-es2015-parameters
```

#### Via Node API

```js
require("babel-core").transform("code", {
  plugins: ["transform-es2015-parameters"]
});
```
