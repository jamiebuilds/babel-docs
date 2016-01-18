# Minify Booleans

### Installation

```sh
$ npm install --save-dev babel-plugin-transform-minify-booleans
```

### Usage

#### Via `.babelrc` (recommended)

**`.babelrc`**

```json
{
  "plugins": ["transform-minify-booleans"]
}
```

#### Via CLI

```sh
babel script.js --plugin transform-minify-booleans
```

#### Via Node API

```js
require("babel-core").transform("code", {
  plugins: ["transform-minify-booleans"]
});
```
