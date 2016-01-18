# Remove Debugger

### Installation

```sh
$ npm install --save-dev babel-plugin-remove-debugger
```

### Usage

#### Via `.babelrc` (recommended)

**`.babelrc`**

```json
{
  "plugins": ["remove-debugger"]
}
```

#### Via CLI

```sh
babel script.js --plugin remove-debugger
```

#### Via Node API

```js
require("babel-core").transform("code", {
  plugins: ["remove-debugger"]
});
```
