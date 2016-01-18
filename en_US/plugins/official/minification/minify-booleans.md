### Installation

```sh
$ npm install --save-dev babel-plugin-minify-booleans
```

### Usage

#### Via `.babelrc` (recommended)

**`.babelrc`**

```json
{
  "plugins": ["minify-booleans"]
}
```

#### Via CLI

```sh
babel script.js --plugin minify-booleans
```

#### Via Node API

```js
require("babel-core").transform("code", {
  plugins: ["minify-booleans"]
});
```
