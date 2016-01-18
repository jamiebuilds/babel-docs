# Regenerator

### Installation

```sh
$ npm install --save-dev babel-plugin-transform-regenerator
```

### Usage

#### Via `.babelrc` (recommended)

**`.babelrc`**

```json
{
  "plugins": ["transform-regenerator"]
}
```

#### Via CLI

```sh
babel script.js --plugin transform-regenerator
```

#### Via Node API

```js
require("babel-core").transform("code", {
  plugins: ["transform-regenerator"]
});
```
