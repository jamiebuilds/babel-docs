# Class Properties

### Installation

```sh
$ npm install --save-dev babel-plugin-class-properties
```

### Usage

#### Via `.babelrc` (recommended)

**`.babelrc`**

```json
{
  "plugins": ["class-properties"]
}
```

#### Via CLI

```sh
babel script.js --plugin class-properties
```

#### Via Node API

```js
require("babel-core").transform("code", {
  plugins: ["class-properties"]
});
```
