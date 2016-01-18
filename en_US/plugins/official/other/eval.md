### Installation

```sh
$ npm install --save-dev babel-plugin-eval
```

### Usage

#### Via `.babelrc` (recommended)

**`.babelrc`**

```json
{
  "plugins": ["eval"]
}
```

#### Via CLI

```sh
babel script.js --plugin eval
```

#### Via Node API

```js
require("babel-core").transform("code", {
  plugins: ["eval"]
});
```
