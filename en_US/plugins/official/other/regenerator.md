### Installation

```sh
$ npm install --save-dev babel-plugin-regenerator
```

### Usage

#### Via `.babelrc` (recommended)

**`.babelrc`**

```json
{
  "plugins": ["regenerator"]
}
```

#### Via CLI

```sh
babel script.js --plugin regenerator
```

#### Via Node API

```js
require("babel-core").transform("code", {
  plugins: ["regenerator"]
});
```
