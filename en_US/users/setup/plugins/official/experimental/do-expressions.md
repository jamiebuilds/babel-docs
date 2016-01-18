# Do Expressions

### Installation

```sh
$ npm install --save-dev babel-plugin-do-expressions
```

### Usage

#### Via `.babelrc` (recommended)

**`.babelrc`**

```json
{
  "plugins": ["do-expressions"]
}
```

#### Via CLI

```sh
babel script.js --plugin do-expressions
```

#### Via Node API

```js
require("babel-core").transform("code", {
  plugins: ["do-expressions"]
});
```
