# Async to Module Method

Compile async functions to Bluebird coroutines

- [GitHub](https://github.com/babel/babel/tree/master/packages/babel-plugin-transform-async-to-module-method)
- [npm](https://www.npmjs.com/package/babel-plugin-transform-async-to-module-method)

## Example

**Input**

```js
async function method() {
  var returned = await asyncFunction();
}
```

**Output**

```js
import { coroutine as _coroutine } from "bluebird";

let method = function () {
  var ref = _coroutine(function* () {
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
$ npm install --save-dev babel-plugin-transform-async-to-module-method
```

### Usage

#### Via `.babelrc` (recommended)

**`.babelrc`**

```json
{
  "plugins": ["transform-async-to-module-method"]
}
```

#### Via CLI

```sh
babel script.js --plugin transform-async-to-module-method
```

#### Via Node API

```js
require("babel-core").transform("code", {
  plugins: ["transform-async-to-module-method"]
});
```
