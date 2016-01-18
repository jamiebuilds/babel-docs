# React JSX Compat

### Installation

```sh
$ npm install --save-dev babel-plugin-transform-react-jsx-compat
```

### Usage

#### Via `.babelrc` (recommended)

**`.babelrc`**

```json
{
  "plugins": ["transform-react-jsx-compat"]
}
```

#### Via CLI

```sh
babel script.js --plugin transform-react-jsx-compat
```

#### Via Node API

```js
require("babel-core").transform("code", {
  plugins: ["transform-react-jsx-compat"]
});
```
