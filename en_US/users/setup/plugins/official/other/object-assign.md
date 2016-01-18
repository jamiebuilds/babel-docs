# Object.assign

### Installation

```sh
$ npm install --save-dev babel-plugin-transform-object-assign
```

### Usage

#### Via `.babelrc` (recommended)

**`.babelrc`**

```json
{
  "plugins": ["transform-object-assign"]
}
```

#### Via CLI

```sh
babel script.js --plugin transform-object-assign
```

#### Via Node API

```js
require("babel-core").transform("code", {
  plugins: ["transform-object-assign"]
});
```
