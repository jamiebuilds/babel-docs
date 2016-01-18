# ES2015 Modules CommonJS

### Installation

```sh
$ npm install --save-dev babel-plugin-es2015-modules-commonjs
```

### Usage

#### Via `.babelrc` (recommended)

**`.babelrc`**

```json
{
  "plugins": ["es2015-modules-commonjs"]
}
```

#### Via CLI

```sh
babel script.js --plugin es2015-modules-commonjs
```

#### Via Node API

```js
require("babel-core").transform("code", {
  plugins: ["es2015-modules-commonjs"]
});
```
