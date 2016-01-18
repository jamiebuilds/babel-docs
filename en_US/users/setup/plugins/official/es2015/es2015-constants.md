# ES2015 Constants

### Installation

```sh
$ npm install --save-dev babel-plugin-es2015-constants
```

### Usage

#### Via `.babelrc` (recommended)

**`.babelrc`**

```json
{
  "plugins": ["es2015-constants"]
}
```

#### Via CLI

```sh
babel script.js --plugin es2015-constants
```

#### Via Node API

```js
require("babel-core").transform("code", {
  plugins: ["es2015-constants"]
});
```
