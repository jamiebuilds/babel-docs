# Remove Console

### Installation

```sh
$ npm install --save-dev babel-plugin-transform-remove-console
```

### Usage

#### Via `.babelrc` (recommended)

**`.babelrc`**

```json
{
  "plugins": ["transform-remove-console"]
}
```

#### Via CLI

```sh
babel script.js --plugin transform-remove-console
```

#### Via Node API

```js
require("babel-core").transform("code", {
  plugins: ["transform-remove-console"]
});
```
