# Simplify Comparison Operators

### Installation

```sh
$ npm install --save-dev babel-plugin-simplify-comparison-operators
```

### Usage

#### Via `.babelrc` (recommended)

**`.babelrc`**

```json
{
  "plugins": ["simplify-comparison-operators"]
}
```

#### Via CLI

```sh
babel script.js --plugin simplify-comparison-operators
```

#### Via Node API

```js
require("babel-core").transform("code", {
  plugins: ["simplify-comparison-operators"]
});
```
