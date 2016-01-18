# Object Rest Spread

### Installation

```sh
$ npm install --save-dev babel-plugin-transform-object-rest-spread
```

### Usage

#### Via `.babelrc` (recommended)

**`.babelrc`**

```json
{
  "plugins": ["transform-object-rest-spread"]
}
```

#### Via CLI

```sh
babel script.js --plugin transform-object-rest-spread
```

#### Via Node API

```js
require("babel-core").transform("code", {
  plugins: ["transform-object-rest-spread"]
});
```
