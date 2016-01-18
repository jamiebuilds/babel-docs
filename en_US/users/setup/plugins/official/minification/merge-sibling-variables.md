# Merge Sibling Variables

### Installation

```sh
$ npm install --save-dev babel-plugin-transform-merge-sibling-variables
```

### Usage

#### Via `.babelrc` (recommended)

**`.babelrc`**

```json
{
  "plugins": ["transform-merge-sibling-variables"]
}
```

#### Via CLI

```sh
babel script.js --plugin transform-merge-sibling-variables
```

#### Via Node API

```js
require("babel-core").transform("code", {
  plugins: ["transform-merge-sibling-variables"]
});
```
