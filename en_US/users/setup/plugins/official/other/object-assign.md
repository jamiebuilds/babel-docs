# Object.assign

### Installation

```sh
$ npm install --save-dev babel-plugin-object-assign
```

### Usage

#### Via `.babelrc` (recommended)

**`.babelrc`**

```json
{
  "plugins": ["object-assign"]
}
```

#### Via CLI

```sh
babel script.js --plugin object-assign
```

#### Via Node API

```js
require("babel-core").transform("code", {
  plugins: ["object-assign"]
});
```
