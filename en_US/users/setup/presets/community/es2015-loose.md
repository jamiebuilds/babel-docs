# ES2015 Loose

### Installation

```sh
$ npm install --save-dev babel-preset-es2015-loose
```

### Usage

#### Via `.babelrc` (recommended)

**`.babelrc`**

```json
{
  "presets": ["es2015-loose"]
}
```

#### Via CLI

```sh
babel script.js --preset es2015-loose
```

#### Via Node API

```js
require("babel-core").transform("code", {
  presets: ["es2015-loose"]
});
```
