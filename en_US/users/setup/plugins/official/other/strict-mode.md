# Strict Mode

### Installation

```sh
$ npm install --save-dev babel-plugin-transform-strict-mode
```

### Usage

#### Via `.babelrc` (recommended)

**`.babelrc`**

```json
{
  "plugins": ["transform-strict-mode"]
}
```

#### Via CLI

```sh
babel script.js --plugin transform-strict-mode
```

#### Via Node API

```js
require("babel-core").transform("code", {
  plugins: ["transform-strict-mode"]
});
```
