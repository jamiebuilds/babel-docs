# Member Expression Literals

### Installation

```sh
$ npm install --save-dev babel-plugin-member-expression-literals
```

### Usage

#### Via `.babelrc` (recommended)

**`.babelrc`**

```json
{
  "plugins": ["member-expression-literals"]
}
```

#### Via CLI

```sh
babel script.js --plugin member-expression-literals
```

#### Via Node API

```js
require("babel-core").transform("code", {
  plugins: ["member-expression-literals"]
});
```
