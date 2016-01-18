# Stage 1

### Installation

```sh
$ npm install --save-dev babel-preset-stage-1
```

### Usage

#### Via `.babelrc` (recommended)

**`.babelrc`**

```json
{
  "presets": ["stage-1"]
}
```

#### Via CLI

```sh
babel script.js --preset stage-1
```

#### Via Node API

```js
require("babel-core").transform("code", {
  presets: ["stage-1"]
});
```
