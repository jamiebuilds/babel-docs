# Undefined to Void

### Installation

```sh
$ npm install --save-dev babel-plugin-transform-undefined-to-void
```

### Usage

#### Via `.babelrc` (recommended)

**`.babelrc`**

```json
{
  "plugins": ["transform-undefined-to-void"]
}
```

#### Via CLI

```sh
babel script.js --plugin transform-undefined-to-void
```

#### Via Node API

```js
require("babel-core").transform("code", {
  plugins: ["transform-undefined-to-void"]
});
```
