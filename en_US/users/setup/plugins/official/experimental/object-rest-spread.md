# Object Rest Spread

Compile object rest and spread to ES5

- [GitHub](https://github.com/babel/babel/tree/master/packages/babel-plugin-transform-object-rest-spread)
- [npm](https://www.npmjs.com/package/babel-plugin-transform-object-rest-spread)

## Example

**Input**

```js
z = { x, ...y };
```

**Output**

```js
z = _extends({ x }, y);
```

> Note that the output may not be exactly what is above. Babel's implementation
> may have changed since this document was last updated, or the output may have
> been cleaned up for clarity.

## Setup

### Installation

```sh
$ npm install --save-dev babel-plugin-transform-object-rest-spread
```

### Usage

#### Via `.babelrc` (recommended)

**`.babelrc`**

```json
{
  "plugins": ["transform-object-rest-spread"]
}
```

#### Via CLI

```sh
babel script.js --plugin transform-object-rest-spread
```

#### Via Node API

```js
require("babel-core").transform("code", {
  plugins: ["transform-object-rest-spread"]
});
```
