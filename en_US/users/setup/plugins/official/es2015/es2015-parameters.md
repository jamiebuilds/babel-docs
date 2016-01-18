# ES2015 Parameters

### Installation

```sh
$ npm install --save-dev babel-plugin-transform-es2015-parameters
```

### Usage

#### Via `.babelrc` (recommended)

**`.babelrc`**

```json
{
  "plugins": ["transform-es2015-parameters"]
}
```

#### Via CLI

```sh
babel script.js --plugin transform-es2015-parameters
```

#### Via Node API

```js
require("babel-core").transform("code", {
  plugins: ["transform-es2015-parameters"]
});
```
