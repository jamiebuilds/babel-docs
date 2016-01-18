# ES2015 Literals

### Installation

```sh
$ npm install --save-dev babel-plugin-transform-es2015-literals
```

### Usage

#### Via `.babelrc` (recommended)

**`.babelrc`**

```json
{
  "plugins": ["transform-es2015-literals"]
}
```

#### Via CLI

```sh
babel script.js --plugin transform-es2015-literals
```

#### Via Node API

```js
require("babel-core").transform("code", {
  plugins: ["transform-es2015-literals"]
});
```
