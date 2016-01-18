### Installation

```sh
$ npm install requirejs-babel
```

### Usage

Add the following paths to your configuration:

```js
paths: {
  es6: "node_modules/requirejs-babel/es6",
  babel: "node_modules/requirejs-babel/babel-4.6.6.min"
}
```

Then reference files via the es6! plugin name:

```js
define(["es6!your-es6-module"], function (module) {
  // ...
});
```

> For more information see the
> [mikach/requirejs-babel repo](https://github.com/mikach/requirejs-babel).
