# Inline Environment Variables

### Installation

```sh
$ npm install --save-dev babel-plugin-transform-inline-environment-variable
```

### Usage

#### Via `.babelrc` (recommended)

**`.babelrc`**

```json
{
  "plugins": ["transform-inline-environment-variable"]
}
```

#### Via CLI

```sh
babel script.js --plugin transform-inline-environment-variable
```

#### Via Node API

```js
require("babel-core").transform("code", {
  plugins: ["transform-inline-environment-variable"]
});
```
