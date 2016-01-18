### Installation

```sh
$ npm install --save-dev babel-plugin-inline-environment-variable
```

### Usage

#### Via `.babelrc` (recommended)

**`.babelrc`**

```json
{
  "plugins": ["inline-environment-variable"]
}
```

#### Via CLI

```sh
babel script.js --plugin inline-environment-variable
```

#### Via Node API

```js
require("babel-core").transform("code", {
  plugins: ["inline-environment-variable"]
});
```
