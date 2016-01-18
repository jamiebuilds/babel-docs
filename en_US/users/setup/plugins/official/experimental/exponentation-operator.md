# Exponentation Operator

### Installation

```sh
$ npm install --save-dev babel-plugin-transform-exponentation-operator
```

### Usage

#### Via `.babelrc` (recommended)

**`.babelrc`**

```json
{
  "plugins": ["transform-exponentation-operator"]
}
```

#### Via CLI

```sh
babel script.js --plugin transform-exponentation-operator
```

#### Via Node API

```js
require("babel-core").transform("code", {
  plugins: ["transform-exponentation-operator"]
});
```
