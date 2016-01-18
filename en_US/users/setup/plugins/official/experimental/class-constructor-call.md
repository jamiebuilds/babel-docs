# Class Constructor Call

### Installation

```sh
$ npm install --save-dev babel-plugin-class-constructor-call
```

### Usage

#### Via `.babelrc` (recommended)

**`.babelrc`**

```json
{
  "plugins": ["class-constructor-call"]
}
```

#### Via CLI

```sh
babel script.js --plugin class-constructor-call
```

#### Via Node API

```js
require("babel-core").transform("code", {
  plugins: ["class-constructor-call"]
});
```
