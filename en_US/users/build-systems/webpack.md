### Installation

```sh
$ npm install --save-dev babel-loader babel-core
```

### Usage

#### Via Config

```js
module: {
  loaders: [
    { test: /\.js$/, exclude: /node_modules/, loader: "babel-loader"}
  ]
}
```

#### Via Loader

```js
var Person = require("babel!./Person.js").default;
new Person();
```

> For more information see the
> [babel/babel-loader repo](https://github.com/babel/babel-loader).
