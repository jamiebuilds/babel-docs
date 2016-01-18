# Function Bind

Compile function bind operator to ES5

## Example

**Input**

```js
ctx::func;
ctx::func();
```

**Output**

```js
var _context;
(_context = ctx, func).bind(_context);

var _context2;
(_context2 = ctx, func).call(_context2);
```

> Note that the output may not be exactly what is above. Babel's implementation
> may have changed since this document was last updated, or the output may have
> been cleaned up for clarity.

## Setup

### Installation

```sh
$ npm install --save-dev babel-plugin-transform-function-bind
```

### Usage

#### Via `.babelrc` (recommended)

**`.babelrc`**

```json
{
  "plugins": ["transform-function-bind"]
}
```

#### Via CLI

```sh
babel script.js --plugin transform-function-bind
```

#### Via Node API

```js
require("babel-core").transform("code", {
  plugins: ["transform-function-bind"]
});
```
