# ES2015 Modules CommonJS

### Installation

```sh
$ npm install --save-dev babel-plugin-transform-es2015-modules-commonjs
```

### Usage

#### Via `.babelrc` (recommended)

**`.babelrc`**

```json
{
  "plugins": ["transform-es2015-modules-commonjs"]
}
```

#### Via CLI

```sh
babel script.js --plugin transform-es2015-modules-commonjs
```

#### Via Node API

```js
require("babel-core").transform("code", {
  plugins: ["transform-es2015-modules-commonjs"]
});
```
