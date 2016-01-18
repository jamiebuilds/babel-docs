# React JSX

### Installation

```sh
$ npm install --save-dev babel-plugin-react-jsx
```

### Usage

#### Via `.babelrc` (recommended)

**`.babelrc`**

```json
{
  "plugins": ["react-jsx"]
}
```

#### Via CLI

```sh
babel script.js --plugin react-jsx
```

#### Via Node API

```js
require("babel-core").transform("code", {
  plugins: ["react-jsx"]
});
```
