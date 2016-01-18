# ES2015 Classes

### Installation

```sh
$ npm install --save-dev babel-plugin-transform-es2015-classes
```

### Usage

#### Via `.babelrc` (recommended)

**`.babelrc`**

```json
{
  "plugins": ["transform-es2015-classes"]
}
```

#### Via CLI

```sh
babel script.js --plugin transform-es2015-classes
```

#### Via Node API

```js
require("babel-core").transform("code", {
  plugins: ["transform-es2015-classes"]
});
```
