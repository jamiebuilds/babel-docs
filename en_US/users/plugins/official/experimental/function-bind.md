### Installation

```sh
$ npm install --save-dev babel-plugin-function-bind
```

### Usage

#### Via `.babelrc` (recommended)

**`.babelrc`**

```json
{
  "plugins": ["function-bind"]
}
```

#### Via CLI

```sh
babel script.js --plugin function-bind
```

#### Via Node API

```js
require("babel-core").transform("code", {
  plugins: ["function-bind"]
});
```
