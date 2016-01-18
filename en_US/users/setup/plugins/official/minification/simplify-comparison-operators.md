# Simplify Comparison Operators

### Installation

```sh
$ npm install --save-dev babel-plugin-transform-simplify-comparison-operators
```

### Usage

#### Via `.babelrc` (recommended)

**`.babelrc`**

```json
{
  "plugins": ["transform-simplify-comparison-operators"]
}
```

#### Via CLI

```sh
babel script.js --plugin transform-simplify-comparison-operators
```

#### Via Node API

```js
require("babel-core").transform("code", {
  plugins: ["transform-simplify-comparison-operators"]
});
```
