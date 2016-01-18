# ES2015 Classes

### Installation

```sh
$ npm install --save-dev babel-plugin-es2015-classes
```

### Usage

#### Via `.babelrc` (recommended)

**`.babelrc`**

```json
{
  "plugins": ["es2015-classes"]
}
```

#### Via CLI

```sh
babel script.js --plugin es2015-classes
```

#### Via Node API

```js
require("babel-core").transform("code", {
  plugins: ["es2015-classes"]
});
```
