# Do Expressions

### Installation

```sh
$ npm install --save-dev babel-plugin-transform-do-expressions
```

### Usage

#### Via `.babelrc` (recommended)

**`.babelrc`**

```json
{
  "plugins": ["transform-do-expressions"]
}
```

#### Via CLI

```sh
babel script.js --plugin transform-do-expressions
```

#### Via Node API

```js
require("babel-core").transform("code", {
  plugins: ["transform-do-expressions"]
});
```
