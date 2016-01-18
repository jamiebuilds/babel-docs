# ES2015 Classes

Compile ES2015 classes to ES5

## Example

**Input**

```js
class Test {
  test() {
    return 5 + 5;
  }
}
```

**Output**

```js
var Test = function () {
  function Test() {
    _classCallCheck(this, Test);
  }

  _createClass(Test, [{
    key: "test",
    value: function test() {
      return 5 + 5;
    }
  }]);

  return Test;
}();
```

> Note that the output may not be exactly what is above. Babel's implementation
> may have changed since this document was last updated, or the output may have
> been cleaned up for clarity.

## Setup

### Installation

```sh
$ npm install --save-dev babel-plugin-transform-es2015-classes
```

### Usage

#### Via `.babelrc` (recommended)

**`.babelrc`**

```json
{
  "plugins": ["transform-es2015-classes"]
}
```

#### Via CLI

```sh
babel script.js --plugin transform-es2015-classes
```

#### Via Node API

```js
require("babel-core").transform("code", {
  plugins: ["transform-es2015-classes"]
});
```
