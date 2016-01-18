# React Display Name

### Installation

```sh
$ npm install --save-dev babel-plugin-transform-react-display-name
```

### Usage

#### Via `.babelrc` (recommended)

**`.babelrc`**

```json
{
  "plugins": ["transform-react-display-name"]
}
```

#### Via CLI

```sh
babel script.js --plugin transform-react-display-name
```

#### Via Node API

```js
require("babel-core").transform("code", {
  plugins: ["transform-react-display-name"]
});
```
