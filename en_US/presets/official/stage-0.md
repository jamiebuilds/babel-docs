### Installation

```sh
$ npm install --save-dev babel-preset-stage-0
```

### Usage

#### Via `.babelrc` (recommended)

**`.babelrc`**

```json
{
  "presets": ["stage-0"]
}
```

#### Via CLI

```sh
babel script.js --preset stage-0
```

#### Via Node API

```js
require("babel-core").transform("code", {
  presets: ["stage-0"]
});
```
