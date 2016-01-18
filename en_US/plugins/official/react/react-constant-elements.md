### Installation

```sh
$ npm install --save-dev babel-plugin-react-constant-elements
```

### Usage

#### Via `.babelrc` (recommended)

**`.babelrc`**

```json
{
  "plugins": ["react-constant-elements"]
}
```

#### Via CLI

```sh
babel script.js --plugin react-constant-elements
```

#### Via Node API

```js
require("babel-core").transform("code", {
  plugins: ["react-constant-elements"]
});
```
