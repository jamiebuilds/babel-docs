# Member Expression Literals

### Installation

```sh
$ npm install --save-dev babel-plugin-transform-member-expression-literals
```

### Usage

#### Via `.babelrc` (recommended)

**`.babelrc`**

```json
{
  "plugins": ["transform-member-expression-literals"]
}
```

#### Via CLI

```sh
babel script.js --plugin transform-member-expression-literals
```

#### Via Node API

```js
require("babel-core").transform("code", {
  plugins: ["transform-member-expression-literals"]
});
```
