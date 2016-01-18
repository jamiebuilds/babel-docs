# ES2015 Node 4

### Installation

```sh
$ npm install --save-dev babel-preset-es2015-node4
```

### Usage

#### Via `.babelrc` (recommended)

**`.babelrc`**

```json
{
  "presets": ["es2015-node4"]
}
```

#### Via CLI

```sh
babel script.js --preset es2015-node4
```

#### Via Node API

```js
require("babel-core").transform("code", {
  presets: ["es2015-node4"]
});
```
