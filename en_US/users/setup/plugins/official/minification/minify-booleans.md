# Minify Booleans

Turn boolean literals into `!0` for `true` and `!1` for `false`.

## Example

**Input**

```js
true;
false;
```

**Output**

```js
!0;
!1;
```

> Note that the output may not be exactly what is above. Babel's implementation
> may have changed since this document was last updated, or the output may have
> been cleaned up for clarity.

## Setup

### Installation

```sh
$ npm install --save-dev babel-plugin-transform-minify-booleans
```

### Usage

#### Via `.babelrc` (recommended)

**`.babelrc`**

```json
{
  "plugins": ["transform-minify-booleans"]
}
```

#### Via CLI

```sh
babel script.js --plugin transform-minify-booleans
```

#### Via Node API

```js
require("babel-core").transform("code", {
  plugins: ["transform-minify-booleans"]
});
```
