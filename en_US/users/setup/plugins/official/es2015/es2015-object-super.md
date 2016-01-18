# ES2015 Object Super

### Installation

```sh
$ npm install --save-dev babel-plugin-transform-es2015-object-super
```

### Usage

#### Via `.babelrc` (recommended)

**`.babelrc`**

```json
{
  "plugins": ["transform-es2015-object-super"]
}
```

#### Via CLI

```sh
babel script.js --plugin transform-es2015-object-super
```

#### Via Node API

```js
require("babel-core").transform("code", {
  plugins: ["transform-es2015-object-super"]
});
```
