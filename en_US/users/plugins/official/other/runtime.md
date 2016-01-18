### Installation

```sh
$ npm install --save-dev babel-plugin-runtime
```

### Usage

#### Via `.babelrc` (recommended)

**`.babelrc`**

```json
{
  "plugins": ["runtime"]
}
```

#### Via CLI

```sh
babel script.js --plugin runtime
```

#### Via Node API

```js
require("babel-core").transform("code", {
  plugins: ["runtime"]
});
```
