# ES2015 Modules UMD

### Installation

```sh
$ npm install --save-dev babel-plugin-transform-es2015-modules-umd
```

### Usage

#### Via `.babelrc` (recommended)

**`.babelrc`**

```json
{
  "plugins": ["transform-es2015-modules-umd"]
}
```

#### Via CLI

```sh
babel script.js --plugin transform-es2015-modules-umd
```

#### Via Node API

```js
require("babel-core").transform("code", {
  plugins: ["transform-es2015-modules-umd"]
});
```
