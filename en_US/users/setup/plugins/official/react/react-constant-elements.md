# React Constant Elements

### Installation

```sh
$ npm install --save-dev babel-plugin-transform-react-constant-elements
```

### Usage

#### Via `.babelrc` (recommended)

**`.babelrc`**

```json
{
  "plugins": ["transform-react-constant-elements"]
}
```

#### Via CLI

```sh
babel script.js --plugin transform-react-constant-elements
```

#### Via Node API

```js
require("babel-core").transform("code", {
  plugins: ["transform-react-constant-elements"]
});
```
