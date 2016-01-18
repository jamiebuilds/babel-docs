# ES2015 Computed Properties

### Installation

```sh
$ npm install --save-dev babel-plugin-transform-es2015-computed-properties
```

### Usage

#### Via `.babelrc` (recommended)

**`.babelrc`**

```json
{
  "plugins": ["transform-es2015-computed-properties"]
}
```

#### Via CLI

```sh
babel script.js --plugin transform-es2015-computed-properties
```

#### Via Node API

```js
require("babel-core").transform("code", {
  plugins: ["transform-es2015-computed-properties"]
});
```
