### Installation

```sh
$ npm install --save-dev babel-preset-stage-2
```

### Usage

#### Via `.babelrc` (recommended)

**`.babelrc`**

```json
{
  "presets": ["stage-2"]
}
```

#### Via CLI

```sh
babel script.js --preset stage-2
```

#### Via Node API

```js
require("babel-core").transform("code", {
  presets: ["stage-2"]
});
```
