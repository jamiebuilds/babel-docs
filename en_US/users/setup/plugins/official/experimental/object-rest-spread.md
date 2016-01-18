# Object Rest Spread

### Installation

```sh
$ npm install --save-dev babel-plugin-object-rest-spread
```

### Usage

#### Via `.babelrc` (recommended)

**`.babelrc`**

```json
{
  "plugins": ["object-rest-spread"]
}
```

#### Via CLI

```sh
babel script.js --plugin object-rest-spread
```

#### Via Node API

```js
require("babel-core").transform("code", {
  plugins: ["object-rest-spread"]
});
```
