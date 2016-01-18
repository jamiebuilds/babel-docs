# Object.setPrototypeOf to Assign

### Installation

```sh
$ npm install --save-dev babel-plugin-object-set-prototype-of-to-assign
```

### Usage

#### Via `.babelrc` (recommended)

**`.babelrc`**

```json
{
  "plugins": ["object-set-prototype-of-to-assign"]
}
```

#### Via CLI

```sh
babel script.js --plugin object-set-prototype-of-to-assign
```

#### Via Node API

```js
require("babel-core").transform("code", {
  plugins: ["object-set-prototype-of-to-assign"]
});
```
