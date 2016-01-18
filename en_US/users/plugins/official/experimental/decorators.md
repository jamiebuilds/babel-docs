### Installation

```sh
$ npm install --save-dev babel-plugin-decorators
```

### Usage

#### Via `.babelrc` (recommended)

**`.babelrc`**

```json
{
  "plugins": ["decorators"]
}
```

#### Via CLI

```sh
babel script.js --plugin decorators
```

#### Via Node API

```js
require("babel-core").transform("code", {
  plugins: ["decorators"]
});
```
