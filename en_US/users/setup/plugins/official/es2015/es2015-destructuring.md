# ES2015 Destructuring

### Installation

```sh
$ npm install --save-dev babel-plugin-es2015-destructuring
```

### Usage

#### Via `.babelrc` (recommended)

**`.babelrc`**

```json
{
  "plugins": ["es2015-destructuring"]
}
```

#### Via CLI

```sh
babel script.js --plugin es2015-destructuring
```

#### Via Node API

```js
require("babel-core").transform("code", {
  plugins: ["es2015-destructuring"]
});
```
