# ES2015 Shorthand Properties

Compile ES2015 shorthand properties to ES5

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
$ npm install --save-dev babel-plugin-transform-es2015-shorthand-properties
```

### Usage

#### Via `.babelrc` (recommended)

**`.babelrc`**

```json
{
  "plugins": ["transform-es2015-shorthand-properties"]
}
```

#### Via CLI

```sh
babel script.js --plugin transform-es2015-shorthand-properties
```

#### Via Node API

```js
require("babel-core").transform("code", {
  plugins: ["transform-es2015-shorthand-properties"]
});
```
