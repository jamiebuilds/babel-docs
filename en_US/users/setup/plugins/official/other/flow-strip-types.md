# Flow Strip Types

### Installation

```sh
$ npm install --save-dev babel-plugin-transform-flow-strip-types
```

### Usage

#### Via `.babelrc` (recommended)

**`.babelrc`**

```json
{
  "plugins": ["transform-flow-strip-types"]
}
```

#### Via CLI

```sh
babel script.js --plugin transform-flow-strip-types
```

#### Via Node API

```js
require("babel-core").transform("code", {
  plugins: ["transform-flow-strip-types"]
});
```
