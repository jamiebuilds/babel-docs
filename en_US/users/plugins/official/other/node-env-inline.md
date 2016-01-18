### Installation

```sh
$ npm install --save-dev babel-plugin-node-env-inline
```

### Usage

#### Via `.babelrc` (recommended)

**`.babelrc`**

```json
{
  "plugins": ["node-env-inline"]
}
```

#### Via CLI

```sh
babel script.js --plugin node-env-inline
```

#### Via Node API

```js
require("babel-core").transform("code", {
  plugins: ["node-env-inline"]
});
```
