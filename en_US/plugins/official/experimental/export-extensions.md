### Installation

```sh
$ npm install --save-dev babel-plugin-export-extensions
```

### Usage

#### Via `.babelrc` (recommended)

**`.babelrc`**

```json
{
  "plugins": ["export-extensions"]
}
```

#### Via CLI

```sh
babel script.js --plugin export-extensions
```

#### Via Node API

```js
require("babel-core").transform("code", {
  plugins: ["export-extensions"]
});
```
