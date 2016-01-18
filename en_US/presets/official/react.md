### Installation

```sh
$ npm install --save-dev babel-preset-react
```

### Usage

#### Via `.babelrc` (recommended)

**`.babelrc`**

```json
{
  "presets": ["react"]
}
```

#### Via CLI

```sh
babel script.js --preset react
```

#### Via Node API

```js
require("babel-core").transform("code", {
  presets: ["react"]
});
```
