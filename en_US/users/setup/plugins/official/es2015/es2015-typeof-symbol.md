# ES2015 typeof Symbol

Ensure `typeof` works with ES2015 Symbols.

## Example

**Input**

```js
typeof s === "symbol"
```

**Output**

```js
(typeof s === "undefined" ? "undefined" : _typeof(s)) === "symbol"
```

> Note that the output may not be exactly what is above. Babel's implementation
> may have changed since this document was last updated, or the output may have
> been cleaned up for clarity.

## Setup

### Installation

```sh
$ npm install --save-dev babel-plugin-transform-es2015-typeof-symbol
```

### Usage

#### Via `.babelrc` (recommended)

**`.babelrc`**

```json
{
  "plugins": ["transform-es2015-typeof-symbol"]
}
```

#### Via CLI

```sh
babel script.js --plugin transform-es2015-typeof-symbol
```

#### Via Node API

```js
require("babel-core").transform("code", {
  plugins: ["transform-es2015-typeof-symbol"]
});
```
