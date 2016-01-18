# Remove Debugger

### Installation

```sh
$ npm install --save-dev babel-plugin-transform-remove-debugger
```

### Usage

#### Via `.babelrc` (recommended)

**`.babelrc`**

```json
{
  "plugins": ["transform-remove-debugger"]
}
```

#### Via CLI

```sh
babel script.js --plugin transform-remove-debugger
```

#### Via Node API

```js
require("babel-core").transform("code", {
  plugins: ["transform-remove-debugger"]
});
```
