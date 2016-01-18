# Property Literals

### Installation

```sh
$ npm install --save-dev babel-plugin-property-literals
```

### Usage

#### Via `.babelrc` (recommended)

**`.babelrc`**

```json
{
  "plugins": ["property-literals"]
}
```

#### Via CLI

```sh
babel script.js --plugin property-literals
```

#### Via Node API

```js
require("babel-core").transform("code", {
  plugins: ["property-literals"]
});
```
