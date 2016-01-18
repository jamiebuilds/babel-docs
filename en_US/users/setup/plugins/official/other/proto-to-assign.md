# Proto to Assign

### Installation

```sh
$ npm install --save-dev babel-plugin-transform-proto-to-assign
```

### Usage

#### Via `.babelrc` (recommended)

**`.babelrc`**

```json
{
  "plugins": ["transform-proto-to-assign"]
}
```

#### Via CLI

```sh
babel script.js --plugin transform-proto-to-assign
```

#### Via Node API

```js
require("babel-core").transform("code", {
  plugins: ["transform-proto-to-assign"]
});
```
