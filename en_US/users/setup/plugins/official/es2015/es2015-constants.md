# ES2015 Constants

### Installation

```sh
$ npm install --save-dev babel-plugin-transform-es2015-constants
```

### Usage

#### Via `.babelrc` (recommended)

**`.babelrc`**

```json
{
  "plugins": ["transform-es2015-constants"]
}
```

#### Via CLI

```sh
babel script.js --plugin transform-es2015-constants
```

#### Via Node API

```js
require("babel-core").transform("code", {
  plugins: ["transform-es2015-constants"]
});
```
