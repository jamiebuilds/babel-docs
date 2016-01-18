### Installation

```sh
$ npm install --save-dev babel-plugin-jscript
```

### Usage

#### Via `.babelrc` (recommended)

**`.babelrc`**

```json
{
  "plugins": ["jscript"]
}
```

#### Via CLI

```sh
babel script.js --plugin jscript
```

#### Via Node API

```js
require("babel-core").transform("code", {
  plugins: ["jscript"]
});
```
