# ES2015 Modules AMD

Convert ES2015 modules to AMD modules

## Example

**Input**

```js
import myModule from "myModule";

export default function() {
  myModule.method();
}
```

**Output**

```js
define(["exports", "myModule"], function (exports, _myModule) {
  "use strict";

  Object.defineProperty(exports, "__esModule", {
    value: true
  });

  var _myModule2 = _interopRequireDefault(_myModule);

  exports.default = function() {
    _myModule2.default.method();
  };
});
```

> Note that the output may not be exactly what is above. Babel's implementation
> may have changed since this document was last updated, or the output may have
> been cleaned up for clarity.

## Setup

### Installation

```sh
$ npm install --save-dev babel-plugin-transform-es2015-modules-amd
```

### Usage

#### Via `.babelrc` (recommended)

**`.babelrc`**

```json
{
  "plugins": ["transform-es2015-modules-amd"]
}
```

#### Via CLI

```sh
babel script.js --plugin transform-es2015-modules-amd
```

#### Via Node API

```js
require("babel-core").transform("code", {
  plugins: ["transform-es2015-modules-amd"]
});
```
