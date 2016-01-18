# Node ENV Inline

### Installation

```sh
$ npm install --save-dev babel-plugin-transform-node-env-inline
```

### Usage

#### Via `.babelrc` (recommended)

**`.babelrc`**

```json
{
  "plugins": ["transform-node-env-inline"]
}
```

#### Via CLI

```sh
babel script.js --plugin transform-node-env-inline
```

#### Via Node API

```js
require("babel-core").transform("code", {
  plugins: ["transform-node-env-inline"]
});
```
