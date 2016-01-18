### Installation

```sh
$ npm install --save-dev babel-plugin-flow-comments
```

### Usage

#### Via `.babelrc` (recommended)

**`.babelrc`**

```json
{
  "plugins": ["flow-comments"]
}
```

#### Via CLI

```sh
babel script.js --plugin flow-comments
```

#### Via Node API

```js
require("babel-core").transform("code", {
  plugins: ["flow-comments"]
});
```
