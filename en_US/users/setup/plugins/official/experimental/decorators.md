# Decorators

> ***THIS PLUGIN HAS NOT YET BEEN IMPLEMENTED. WAITING ON THE UPDATED PROPOSAL***

### Installation

```sh
$ npm install --save-dev babel-plugin-transform-decorators
```

### Usage

#### Via `.babelrc` (recommended)

**`.babelrc`**

```json
{
  "plugins": ["transform-decorators"]
}
```

#### Via CLI

```sh
babel script.js --plugin transform-decorators
```

#### Via Node API

```js
require("babel-core").transform("code", {
  plugins: ["transform-decorators"]
});
```
