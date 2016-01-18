# ES2015 Sticky Regex

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
