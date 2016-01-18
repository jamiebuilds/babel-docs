### Installation

```sh
$ npm install --save-dev rollup
$ npm install --save-dev rollup-plugin-babel
```

### Usage

```js
var rollup = require("rollup");
var babel = require("rollup-plugin-babel");

rollup.rollup({
  entry: "src/main.js",
  plugins: [babel()]
}).then(function (bundle) {
  bundle.write({
    dest: "dist/bundle.js",
    format: "umd"
  });
});
```

> For more information see the [rollup](https://github.com/rollup/rollup) and
> [rollup-plugin-babel](https://github.com/rollup/rollup-plugin-babel) repos.
