### Installation

```sh
$ npm install --save-dev babel-plugin-es2015-unicode-regex
```

### Usage

#### Via `.babelrc` (recommended)

**`.babelrc`**

```json
{
  "plugins": ["es2015-unicode-regex"]
}
```

#### Via CLI

```sh
babel script.js --plugin es2015-unicode-regex
```

#### Via Node API

```js
require("babel-core").transform("code", {
  plugins: ["es2015-unicode-regex"]
});
```
