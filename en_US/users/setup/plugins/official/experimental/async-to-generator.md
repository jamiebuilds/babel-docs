# Async to Generator

## Example

**Input**

```js
async function method() {
  var returned = await asyncFunction();
}
```

**Output**

```js
let method = function () {
  var ref = _asyncToGenerator(function* () {
    var returned = yield asyncFunction();
  });
  return function method() {
    return ref.apply(this, arguments);
  };
}();
```

> Note that the output may not be exactly what is above. Babel's implementation
> may have changed since this document was last updated, or the output may have
> been cleaned up for clarity.

## Setup

### Installation

```sh
$ npm install --save-dev babel-plugin-transform-async-to-generator
```

### Usage

#### Via `.babelrc` (recommended)

**`.babelrc`**

```json
{
  "plugins": ["transform-async-to-generator"]
}
```

#### Via CLI

```sh
babel script.js --plugin transform-async-to-generator
```

#### Via Node API

```js
require("babel-core").transform("code", {
  plugins: ["transform-async-to-generator"]
});
```
