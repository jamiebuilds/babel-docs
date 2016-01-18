# Property Literals

### Installation

```sh
$ npm install --save-dev babel-plugin-transform-property-literals
```

### Usage

#### Via `.babelrc` (recommended)

**`.babelrc`**

```json
{
  "plugins": ["transform-property-literals"]
}
```

#### Via CLI

```sh
babel script.js --plugin transform-property-literals
```

#### Via Node API

```js
require("babel-core").transform("code", {
  plugins: ["transform-property-literals"]
});
```
