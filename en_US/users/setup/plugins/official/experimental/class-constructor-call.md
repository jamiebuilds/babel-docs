# Class Constructor Call

Compile class call constructors to ES2015

## Example

**Input**

```js
class MyClass {
  call constructor() {
    method();
  }
}
```

**Output**

```js
let _MyClass = class MyClass {};

var _MyClassCall = function () {
  method();
};

var MyClass = function (...args) {
  if (this instanceof MyClass) {
    return Reflect.construct(_MyClass, args);
  } else {
    return _MyClassCall.apply(this, args);
  }
};

MyClass.__proto__ = _MyClass;
MyClass;
```

> Note that the output may not be exactly what is above. Babel's implementation
> may have changed since this document was last updated, or the output may have
> been cleaned up for clarity.

## Setup

### Installation

```sh
$ npm install --save-dev babel-plugin-transform-class-constructor-call
```

### Usage

#### Via `.babelrc` (recommended)

**`.babelrc`**

```json
{
  "plugins": ["transform-class-constructor-call"]
}
```

#### Via CLI

```sh
babel script.js --plugin transform-class-constructor-call
```

#### Via Node API

```js
require("babel-core").transform("code", {
  plugins: ["transform-class-constructor-call"]
});
```
