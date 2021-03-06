# ES2015 Spread

Compile ES2015 spread to ES5

## Example

**Input**

```js
[a, ...b, c];
```

**Output**

```js
[a].concat(_toConsumableArray(b), [c]);
```

> Note that the output may not be exactly what is above. Babel's implementation
> may have changed since this document was last updated, or the output may have
> been cleaned up for clarity.

## Setup

### Installation

```sh
$ npm install --save-dev babel-plugin-transform-es2015-spread
```

### Usage

#### Via `.babelrc` (recommended)

**`.babelrc`**

```json
{
  "plugins": ["transform-es2015-spread"]
}
```

#### Via CLI

```sh
babel script.js --plugin transform-es2015-spread
```

#### Via Node API

```js
require("babel-core").transform("code", {
  plugins: ["transform-es2015-spread"]
});
```
