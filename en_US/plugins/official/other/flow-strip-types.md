### Installation

```sh
$ npm install --save-dev babel-plugin-flow-strip-types
```

### Usage

#### Via `.babelrc` (recommended)

**`.babelrc`**

```json
{
  "plugins": ["flow-strip-types"]
}
```

#### Via CLI

```sh
babel script.js --plugin flow-strip-types
```

#### Via Node API

```js
require("babel-core").transform("code", {
  plugins: ["flow-strip-types"]
});
```
