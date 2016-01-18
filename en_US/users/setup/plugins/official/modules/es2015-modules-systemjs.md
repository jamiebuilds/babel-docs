# ES2015 Modules SystemJS

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
$ npm install --save-dev babel-plugin-transform-es2015-modules-systemjs
```

### Usage

#### Via `.babelrc` (recommended)

**`.babelrc`**

```json
{
  "plugins": ["transform-es2015-modules-systemjs"]
}
```

#### Via CLI

```sh
babel script.js --plugin transform-es2015-modules-systemjs
```

#### Via Node API

```js
require("babel-core").transform("code", {
  plugins: ["transform-es2015-modules-systemjs"]
});
```
