# Broccoli

### Installation

```sh
$ npm install --save-dev broccoli-babel-transpiler
```

### Usage

Inside of your `Brocfile.js` add the following:

```js
var babelTranspiler = require("broccoli-babel-transpiler");
var scriptTree = babelTranspiler(inputTree, options);
```

> For more information see the
> [babel/broccoli-babel-transpiler repo](https://github.com/babel/broccoli-babel-transpiler).
