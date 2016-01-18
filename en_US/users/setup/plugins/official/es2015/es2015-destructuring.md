# ES2015 Destructuring

Compile ES2015 destructuring to ES5

## Example

**Input**

```js
const coords = { x: 1, y: 2 };
const { x, y } = coords;
```

**Output**

```js
const coords = { x: 1, y: 2 };
const x = coords.x;
const y = coords.y;
```

> Note that the output may not be exactly what is above. Babel's implementation
> may have changed since this document was last updated, or the output may have
> been cleaned up for clarity.

## Setup

### Installation

```sh
$ npm install --save-dev babel-plugin-transform-es2015-destructuring
```

### Usage

#### Via `.babelrc` (recommended)

**`.babelrc`**

```json
{
  "plugins": ["transform-es2015-destructuring"]
}
```

#### Via CLI

```sh
babel script.js --plugin transform-es2015-destructuring
```

#### Via Node API

```js
require("babel-core").transform("code", {
  plugins: ["transform-es2015-destructuring"]
});
```
