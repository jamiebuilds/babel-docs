# React Inline Elements

### Installation

```sh
$ npm install --save-dev babel-plugin-react-inline-elements
```

### Usage

#### Via `.babelrc` (recommended)

**`.babelrc`**

```json
{
  "plugins": ["react-inline-elements"]
}
```

#### Via CLI

```sh
babel script.js --plugin react-inline-elements
```

#### Via Node API

```js
require("babel-core").transform("code", {
  plugins: ["react-inline-elements"]
});
```
