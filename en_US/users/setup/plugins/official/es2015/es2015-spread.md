# ES2015 Spread

### Installation

```sh
$ npm install --save-dev babel-plugin-transform-es2015-spread
```

### Usage

#### Via `.babelrc` (recommended)

**`.babelrc`**

```json
{
  "plugins": ["transform-es2015-spread"]
}
```

#### Via CLI

```sh
babel script.js --plugin transform-es2015-spread
```

#### Via Node API

```js
require("babel-core").transform("code", {
  plugins: ["transform-es2015-spread"]
});
```
