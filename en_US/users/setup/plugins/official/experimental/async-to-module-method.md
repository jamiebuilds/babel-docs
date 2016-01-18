# Async to Module Method

### Installation

```sh
$ npm install --save-dev babel-plugin-async-to-module-method
```

### Usage

#### Via `.babelrc` (recommended)

**`.babelrc`**

```json
{
  "plugins": ["async-to-module-method"]
}
```

#### Via CLI

```sh
babel script.js --plugin async-to-module-method
```

#### Via Node API

```js
require("babel-core").transform("code", {
  plugins: ["async-to-module-method"]
});
```
