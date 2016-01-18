# Remove Console

### Installation

```sh
$ npm install --save-dev babel-plugin-remove-console
```

### Usage

#### Via `.babelrc` (recommended)

**`.babelrc`**

```json
{
  "plugins": ["remove-console"]
}
```

#### Via CLI

```sh
babel script.js --plugin remove-console
```

#### Via Node API

```js
require("babel-core").transform("code", {
  plugins: ["remove-console"]
});
```
