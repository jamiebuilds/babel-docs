# Runtime

### Installation

```sh
$ npm install --save-dev babel-plugin-transform-runtime
```

### Usage

#### Via `.babelrc` (recommended)

**`.babelrc`**

```json
{
  "plugins": ["transform-runtime"]
}
```

#### Via CLI

```sh
babel script.js --plugin transform-runtime
```

#### Via Node API

```js
require("babel-core").transform("code", {
  plugins: ["transform-runtime"]
});
```
