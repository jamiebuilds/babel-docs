### Installation

```sh
$ npm install --save-dev babel-plugin-proto-to-assign
```

### Usage

#### Via `.babelrc` (recommended)

**`.babelrc`**

```json
{
  "plugins": ["proto-to-assign"]
}
```

#### Via CLI

```sh
babel script.js --plugin proto-to-assign
```

#### Via Node API

```js
require("babel-core").transform("code", {
  plugins: ["proto-to-assign"]
});
```
