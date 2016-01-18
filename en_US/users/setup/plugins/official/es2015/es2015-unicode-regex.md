# ES2015 Unicode Regex

Compile ES2015 unicode regex to ES5

## Example

**Input**

```js
var string = "foo💩bar";
var match = string.match(/foo(.)bar/u);
```

**Output**

```js
var string = "foo💩bar";
var match = string.match(/foo((?:[\0-\t\x0B\f\x0E-\u2027\u202A-\uD7FF\uE000-\uFFFF]|[\uD800-\uDBFF][\uDC00-\uDFFF]|[\uD800-\uDBFF](?![\uDC00-\uDFFF])|(?:[^\uD800-\uDBFF]|^)[\uDC00-\uDFFF]))bar/);
```

> Note that the output may not be exactly what is above. Babel's implementation
> may have changed since this document was last updated, or the output may have
> been cleaned up for clarity.

## Setup

### Installation

```sh
$ npm install --save-dev babel-plugin-transform-es2015-unicode-regex
```

### Usage

#### Via `.babelrc` (recommended)

**`.babelrc`**

```json
{
  "plugins": ["transform-es2015-unicode-regex"]
}
```

#### Via CLI

```sh
babel script.js --plugin transform-es2015-unicode-regex
```

#### Via Node API

```js
require("babel-core").transform("code", {
  plugins: ["transform-es2015-unicode-regex"]
});
```
