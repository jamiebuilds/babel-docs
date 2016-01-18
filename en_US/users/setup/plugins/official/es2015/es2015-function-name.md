# ES2015 Function Name

### Installation

```sh
$ npm install --save-dev babel-plugin-transform-es2015-function-name
```

### Usage

#### Via `.babelrc` (recommended)

**`.babelrc`**

```json
{
  "plugins": ["transform-es2015-function-name"]
}
```

#### Via CLI

```sh
babel script.js --plugin transform-es2015-function-name
```

#### Via Node API

```js
require("babel-core").transform("code", {
  plugins: ["transform-es2015-function-name"]
});
```
