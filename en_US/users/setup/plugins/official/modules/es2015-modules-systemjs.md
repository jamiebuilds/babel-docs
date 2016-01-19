# ES2015 Modules SystemJS

Convert ES2015 modules to SystemJS modules

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
System.register(["myModule"], function (_export, _context) {
  var myModule;

  _export("default", function () {
    myModule.method();
  });

  return {
    setters: [function(_myModule) {
      myModule = _myModule.default;
    }],
    execute: function () {
      _export("default", foo);
    }
  };
});
```

> Note that the output may not be exactly what is above. Babel's implementation
> may have changed since this document was last updated, or the output may have
> been cleaned up for clarity.

## Setup

### Installation

```sh
$ npm install --save-dev babel-plugin-transform-es2015-modules-systemjs
```

### Usage

#### Via `.babelrc` (recommended)

**`.babelrc`**

```json
{
  "plugins": ["transform-es2015-modules-systemjs"]
}
```

#### Via CLI

```sh
babel script.js --plugin transform-es2015-modules-systemjs
```

#### Via Node API

```js
require("babel-core").transform("code", {
  plugins: ["transform-es2015-modules-systemjs"]
});
```
