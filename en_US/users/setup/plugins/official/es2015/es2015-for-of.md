# ES2015 For Of

### Installation

```sh
$ npm install --save-dev babel-plugin-es2015-for-of
```

### Usage

#### Via `.babelrc` (recommended)

**`.babelrc`**

```json
{
  "plugins": ["es2015-for-of"]
}
```

#### Via CLI

```sh
babel script.js --plugin es2015-for-of
```

#### Via Node API

```js
require("babel-core").transform("code", {
  plugins: ["es2015-for-of"]
});
```
