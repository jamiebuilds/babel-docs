# ES2015 Shorthand Properties

### Installation

```sh
$ npm install --save-dev babel-plugin-transform-es2015-shorthand-properties
```

### Usage

#### Via `.babelrc` (recommended)

**`.babelrc`**

```json
{
  "plugins": ["transform-es2015-shorthand-properties"]
}
```

#### Via CLI

```sh
babel script.js --plugin transform-es2015-shorthand-properties
```

#### Via Node API

```js
require("babel-core").transform("code", {
  plugins: ["transform-es2015-shorthand-properties"]
});
```
