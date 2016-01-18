# Object.setPrototypeOf to Assign

### Installation

```sh
$ npm install --save-dev babel-plugin-transform-object-set-prototype-of-to-assign
```

### Usage

#### Via `.babelrc` (recommended)

**`.babelrc`**

```json
{
  "plugins": ["transform-object-set-prototype-of-to-assign"]
}
```

#### Via CLI

```sh
babel script.js --plugin transform-object-set-prototype-of-to-assign
```

#### Via Node API

```js
require("babel-core").transform("code", {
  plugins: ["transform-object-set-prototype-of-to-assign"]
});
```
