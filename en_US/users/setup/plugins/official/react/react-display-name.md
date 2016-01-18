# React Display Name

### Installation

```sh
$ npm install --save-dev babel-plugin-react-display-name
```

### Usage

#### Via `.babelrc` (recommended)

**`.babelrc`**

```json
{
  "plugins": ["react-display-name"]
}
```

#### Via CLI

```sh
babel script.js --plugin react-display-name
```

#### Via Node API

```js
require("babel-core").transform("code", {
  plugins: ["react-display-name"]
});
```
