# JScript

### Installation

```sh
$ npm install --save-dev babel-plugin-transform-jscript
```

### Usage

#### Via `.babelrc` (recommended)

**`.babelrc`**

```json
{
  "plugins": ["transform-jscript"]
}
```

#### Via CLI

```sh
babel script.js --plugin transform-jscript
```

#### Via Node API

```js
require("babel-core").transform("code", {
  plugins: ["transform-jscript"]
});
```
