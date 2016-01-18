# Function Bind

### Installation

```sh
$ npm install --save-dev babel-plugin-transform-function-bind
```

### Usage

#### Via `.babelrc` (recommended)

**`.babelrc`**

```json
{
  "plugins": ["transform-function-bind"]
}
```

#### Via CLI

```sh
babel script.js --plugin transform-function-bind
```

#### Via Node API

```js
require("babel-core").transform("code", {
  plugins: ["transform-function-bind"]
});
```
