# Async to Generator

### Installation

```sh
$ npm install --save-dev babel-plugin-async-to-generator
```

### Usage

#### Via `.babelrc` (recommended)

**`.babelrc`**

```json
{
  "plugins": ["async-to-generator"]
}
```

#### Via CLI

```sh
babel script.js --plugin async-to-generator
```

#### Via Node API

```js
require("babel-core").transform("code", {
  plugins: ["async-to-generator"]
});
```
