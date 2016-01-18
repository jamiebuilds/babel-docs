# ES2015 Block Scoped Functions

### Installation

```sh
$ npm install --save-dev babel-plugin-transform-es2015-block-scoped-functions
```

### Usage

#### Via `.babelrc` (recommended)

**`.babelrc`**

```json
{
  "plugins": ["transform-es2015-block-scoped-functions"]
}
```

#### Via CLI

```sh
babel script.js --plugin transform-es2015-block-scoped-functions
```

#### Via Node API

```js
require("babel-core").transform("code", {
  plugins: ["transform-es2015-block-scoped-functions"]
});
```
