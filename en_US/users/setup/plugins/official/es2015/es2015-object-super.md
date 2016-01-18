# ES2015 Object super

Compile ES2015 object super to ES5

## Example

**Input**

```js
var obj = {
  method() {
    return super.prop;
  }
};
```

**Output**

```js
var _obj;

var obj = _obj = {
  method: function () {
    return _get(Object.getPrototypeOf(_obj), "prop", this);
  }
};
```

> Note that the output may not be exactly what is above. Babel's implementation
> may have changed since this document was last updated, or the output may have
> been cleaned up for clarity.

## Setup

### Installation

```sh
$ npm install --save-dev babel-plugin-transform-es2015-object-super
```

### Usage

#### Via `.babelrc` (recommended)

**`.babelrc`**

```json
{
  "plugins": ["transform-es2015-object-super"]
}
```

#### Via CLI

```sh
babel script.js --plugin transform-es2015-object-super
```

#### Via Node API

```js
require("babel-core").transform("code", {
  plugins: ["transform-es2015-object-super"]
});
```
