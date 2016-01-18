# Export Extensions

Compile export extensions to ES2015

- [GitHub](https://github.com/babel/babel/tree/master/packages/babel-plugin-transform-export-extensions)
- [npm](https://www.npmjs.com/package/babel-plugin-transform-export-extensions)

## Example

**Input**

```js
export foo from "bar";
export * as foo from "bar";
export v, { x, y as w } from "mod";
```

**Output**

```js
import _foo from "bar";
export { _foo as foo };

import * as _foo from "bar";
export { _foo as foo };

import _v from "mod";
export { _v as v };
export { x, y as w } from "mod";
```

> Note that the output may not be exactly what is above. Babel's implementation
> may have changed since this document was last updated, or the output may have
> been cleaned up for clarity.

## Setup

### Installation

```sh
$ npm install --save-dev babel-plugin-transform-export-extensions
```

### Usage

#### Via `.babelrc` (recommended)

**`.babelrc`**

```json
{
  "plugins": ["transform-export-extensions"]
}
```

#### Via CLI

```sh
babel script.js --plugin transform-export-extensions
```

#### Via Node API

```js
require("babel-core").transform("code", {
  plugins: ["transform-export-extensions"]
});
```
