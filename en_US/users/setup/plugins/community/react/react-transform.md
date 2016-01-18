# React Transform

### Installation

```sh
$ npm install --save-dev babel-plugin-react-transform
```

### Usage

#### Via `.babelrc` (recommended)

**`.babelrc`**

```json
{
  "plugins": ["react-transform"]
}
```

#### Via CLI

```sh
babel script.js --plugin react-transform
```

#### Via Node API

```js
require("babel-core").transform("code", {
  plugins: ["react-transform"]
});
```
