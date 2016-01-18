# ES2015 Parameters

### Installation

```sh
$ npm install --save-dev babel-plugin-es2015-parameters
```

### Usage

#### Via `.babelrc` (recommended)

**`.babelrc`**

```json
{
  "plugins": ["es2015-parameters"]
}
```

#### Via CLI

```sh
babel script.js --plugin es2015-parameters
```

#### Via Node API

```js
require("babel-core").transform("code", {
  plugins: ["es2015-parameters"]
});
```
