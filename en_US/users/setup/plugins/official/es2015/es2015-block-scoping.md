# ES2015 Block Scoping

### Installation

```sh
$ npm install --save-dev babel-plugin-transform-es2015-block-scoping
```

### Usage

#### Via `.babelrc` (recommended)

**`.babelrc`**

```json
{
  "plugins": ["transform-es2015-block-scoping"]
}
```

#### Via CLI

```sh
babel script.js --plugin transform-es2015-block-scoping
```

#### Via Node API

```js
require("babel-core").transform("code", {
  plugins: ["transform-es2015-block-scoping"]
});
```
