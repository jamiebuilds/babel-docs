# ES2015 Modules AMD

### Installation

```sh
$ npm install --save-dev babel-plugin-es2015-modules-amd
```

### Usage

#### Via `.babelrc` (recommended)

**`.babelrc`**

```json
{
  "plugins": ["es2015-modules-amd"]
}
```

#### Via CLI

```sh
babel script.js --plugin es2015-modules-amd
```

#### Via Node API

```js
require("babel-core").transform("code", {
  plugins: ["es2015-modules-amd"]
});
```
