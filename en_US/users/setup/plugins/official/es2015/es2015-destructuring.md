# ES2015 Destructuring

### Installation

```sh
$ npm install --save-dev babel-plugin-transform-es2015-destructuring
```

### Usage

#### Via `.babelrc` (recommended)

**`.babelrc`**

```json
{
  "plugins": ["transform-es2015-destructuring"]
}
```

#### Via CLI

```sh
babel script.js --plugin transform-es2015-destructuring
```

#### Via Node API

```js
require("babel-core").transform("code", {
  plugins: ["transform-es2015-destructuring"]
});
```
