# Export Extensions

### Installation

```sh
$ npm install --save-dev babel-plugin-transform-export-extensions
```

### Usage

#### Via `.babelrc` (recommended)

**`.babelrc`**

```json
{
  "plugins": ["transform-export-extensions"]
}
```

#### Via CLI

```sh
babel script.js --plugin transform-export-extensions
```

#### Via Node API

```js
require("babel-core").transform("code", {
  plugins: ["transform-export-extensions"]
});
```
