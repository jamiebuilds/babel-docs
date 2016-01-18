# ES2015 Constants

Validate ES2015 constants

## Example

**Input**

```js
```

**Output**

```js
```

> Note that the output may not be exactly what is above. Babel's implementation
> may have changed since this document was last updated, or the output may have
> been cleaned up for clarity.

## Setup

### Installation

```sh
$ npm install --save-dev babel-plugin-check-es2015-constants
```

### Usage

#### Via `.babelrc` (recommended)

**`.babelrc`**

```json
{
  "plugins": ["check-es2015-constants"]
}
```

#### Via CLI

```sh
babel script.js --plugin check-es2015-constants
```

#### Via Node API

```js
require("babel-core").check("code", {
  plugins: ["check-es2015-constants"]
});
```
