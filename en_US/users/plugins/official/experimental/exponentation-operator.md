### Installation

```sh
$ npm install --save-dev babel-plugin-exponentation-operator
```

### Usage

#### Via `.babelrc` (recommended)

**`.babelrc`**

```json
{
  "plugins": ["exponentation-operator"]
}
```

#### Via CLI

```sh
babel script.js --plugin exponentation-operator
```

#### Via Node API

```js
require("babel-core").transform("code", {
  plugins: ["exponentation-operator"]
});
```
