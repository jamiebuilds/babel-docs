# ES2015 Modules SystemJS

### Installation

```sh
$ npm install --save-dev babel-plugin-transform-es2015-modules-systemjs
```

### Usage

#### Via `.babelrc` (recommended)

**`.babelrc`**

```json
{
  "plugins": ["transform-es2015-modules-systemjs"]
}
```

#### Via CLI

```sh
babel script.js --plugin transform-es2015-modules-systemjs
```

#### Via Node API

```js
require("babel-core").transform("code", {
  plugins: ["transform-es2015-modules-systemjs"]
});
```
