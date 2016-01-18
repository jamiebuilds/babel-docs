# Eval

### Installation

```sh
$ npm install --save-dev babel-plugin-transform-eval
```

### Usage

#### Via `.babelrc` (recommended)

**`.babelrc`**

```json
{
  "plugins": ["transform-eval"]
}
```

#### Via CLI

```sh
babel script.js --plugin transform-eval
```

#### Via Node API

```js
require("babel-core").transform("code", {
  plugins: ["transform-eval"]
});
```
