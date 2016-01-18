# Flow Comments

### Installation

```sh
$ npm install --save-dev babel-plugin-transform-flow-comments
```

### Usage

#### Via `.babelrc` (recommended)

**`.babelrc`**

```json
{
  "plugins": ["transform-flow-comments"]
}
```

#### Via CLI

```sh
babel script.js --plugin transform-flow-comments
```

#### Via Node API

```js
require("babel-core").transform("code", {
  plugins: ["transform-flow-comments"]
});
```
