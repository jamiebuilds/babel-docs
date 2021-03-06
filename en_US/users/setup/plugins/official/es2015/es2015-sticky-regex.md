# ES2015 Sticky Regex

Compile ES2015 sticky regex to an ES5 RegExp constructor

## Example

**Input**

```js
/o+/y;
```

**Output**

```js
new RegExp("o+", "y");
```

> Note that the output may not be exactly what is above. Babel's implementation
> may have changed since this document was last updated, or the output may have
> been cleaned up for clarity.

## Setup

### Installation

```sh
$ npm install --save-dev babel-plugin-transform-es2015-sticky-regex
```

### Usage

#### Via `.babelrc` (recommended)

**`.babelrc`**

```json
{
  "plugins": ["transform-es2015-sticky-regex"]
}
```

#### Via CLI

```sh
babel script.js --plugin transform-es2015-sticky-regex
```

#### Via Node API

```js
require("babel-core").transform("code", {
  plugins: ["transform-es2015-sticky-regex"]
});
```
