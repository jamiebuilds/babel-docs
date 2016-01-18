# ES2015 Unicode Regex

### Installation

```sh
$ npm install --save-dev babel-plugin-transform-es2015-unicode-regex
```

### Usage

#### Via `.babelrc` (recommended)

**`.babelrc`**

```json
{
  "plugins": ["transform-es2015-unicode-regex"]
}
```

#### Via CLI

```sh
babel script.js --plugin transform-es2015-unicode-regex
```

#### Via Node API

```js
require("babel-core").transform("code", {
  plugins: ["transform-es2015-unicode-regex"]
});
```
