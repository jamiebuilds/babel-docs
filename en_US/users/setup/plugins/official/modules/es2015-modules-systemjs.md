# ES2015 Modules SystemJS

### Installation

```sh
$ npm install --save-dev babel-plugin-es2015-modules-systemjs
```

### Usage

#### Via `.babelrc` (recommended)

**`.babelrc`**

```json
{
  "plugins": ["es2015-modules-systemjs"]
}
```

#### Via CLI

```sh
babel script.js --plugin es2015-modules-systemjs
```

#### Via Node API

```js
require("babel-core").transform("code", {
  plugins: ["es2015-modules-systemjs"]
});
```
