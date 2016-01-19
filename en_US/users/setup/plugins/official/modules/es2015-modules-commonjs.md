# ES2015 Modules CommonJS

Convert ES2015 modules to CommonJS modules

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
var _myModule = require("myModule");
var _myModule2 = _interopRequireDefault(_myModule);

exports.default = function() {
  _myModule2.default.method();
};
```

> Note that the output may not be exactly what is above. Babel's implementation
> may have changed since this document was last updated, or the output may have
> been cleaned up for clarity.

## Setup

### Installation

```sh
$ npm install --save-dev babel-plugin-transform-es2015-modules-commonjs
```

### Usage

#### Via `.babelrc` (recommended)

**`.babelrc`**

```json
{
  "plugins": ["transform-es2015-modules-commonjs"]
}
```

#### Via CLI

```sh
babel script.js --plugin transform-es2015-modules-commonjs
```

#### Via Node API

```js
require("babel-core").transform("code", {
  plugins: ["transform-es2015-modules-commonjs"]
});
```
