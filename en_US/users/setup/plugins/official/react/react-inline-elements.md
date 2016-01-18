# React Inline Elements

### Installation

```sh
$ npm install --save-dev babel-plugin-transform-react-inline-elements
```

### Usage

#### Via `.babelrc` (recommended)

**`.babelrc`**

```json
{
  "plugins": ["transform-react-inline-elements"]
}
```

#### Via CLI

```sh
babel script.js --plugin transform-react-inline-elements
```

#### Via Node API

```js
require("babel-core").transform("code", {
  plugins: ["transform-react-inline-elements"]
});
```
