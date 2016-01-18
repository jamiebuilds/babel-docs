# Stage 3

### Installation

```sh
$ npm install --save-dev babel-preset-stage-3
```

### Usage

#### Via `.babelrc` (recommended)

**`.babelrc`**

```json
{
  "presets": ["stage-3"]
}
```

#### Via CLI

```sh
babel script.js --preset stage-3
```

#### Via Node API

```js
require("babel-core").transform("code", {
  presets: ["stage-3"]
});
```
