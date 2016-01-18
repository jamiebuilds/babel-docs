# React JSX Compat

### Installation

```sh
$ npm install --save-dev babel-plugin-react-jsx-compat
```

### Usage

#### Via `.babelrc` (recommended)

**`.babelrc`**

```json
{
  "plugins": ["react-jsx-compat"]
}
```

#### Via CLI

```sh
babel script.js --plugin react-jsx-compat
```

#### Via Node API

```js
require("babel-core").transform("code", {
  plugins: ["react-jsx-compat"]
});
```
