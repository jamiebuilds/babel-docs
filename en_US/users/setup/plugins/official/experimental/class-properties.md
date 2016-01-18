# Class Properties

Compile static and instance class properties to ES2015

- [GitHub](https://github.com/babel/babel/tree/master/packages/babel-plugin-transform-class-properties)
- [npm](https://www.npmjs.com/package/babel-plugin-transform-class-properties)

## Example

**Input**

```js
class MyClass {
  static property = "value";
  property = "value";
}
```

**Output**

```js
class MyClass {
  constructor() {
    this.property = "value";
  }
}
MyClass.property = "value";
```

> Note that the output may not be exactly what is above. Babel's implementation
> may have changed since this document was last updated, or the output may have
> been cleaned up for clarity.

## Setup

### Installation

```sh
$ npm install --save-dev babel-plugin-transform-class-properties
```

### Usage

#### Via `.babelrc` (recommended)

**`.babelrc`**

```json
{
  "plugins": ["transform-class-properties"]
}
```

#### Via CLI

```sh
babel script.js --plugin transform-class-properties
```

#### Via Node API

```js
require("babel-core").transform("code", {
  plugins: ["transform-class-properties"]
});
```
