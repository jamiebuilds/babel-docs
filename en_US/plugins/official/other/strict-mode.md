### Installation

```sh
$ npm install --save-dev babel-plugin-strict-mode
```

### Usage

#### Via `.babelrc` (recommended)

**`.babelrc`**

```json
{
  "plugins": ["strict-mode"]
}
```

#### Via CLI

```sh
babel script.js --plugin strict-mode
```

#### Via Node API

```js
require("babel-core").transform("code", {
  plugins: ["strict-mode"]
});
```
