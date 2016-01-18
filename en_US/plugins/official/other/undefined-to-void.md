### Installation

```sh
$ npm install --save-dev babel-plugin-undefined-to-void
```

### Usage

#### Via `.babelrc` (recommended)

**`.babelrc`**

```json
{
  "plugins": ["undefined-to-void"]
}
```

#### Via CLI

```sh
babel script.js --plugin undefined-to-void
```

#### Via Node API

```js
require("babel-core").transform("code", {
  plugins: ["undefined-to-void"]
});
```
