# React JSX

### Installation

```sh
$ npm install --save-dev babel-plugin-transform-react-jsx
```

### Usage

#### Via `.babelrc` (recommended)

**`.babelrc`**

```json
{
  "plugins": ["transform-react-jsx"]
}
```

#### Via CLI

```sh
babel script.js --plugin transform-react-jsx
```

#### Via Node API

```js
require("babel-core").transform("code", {
  plugins: ["transform-react-jsx"]
});
```
