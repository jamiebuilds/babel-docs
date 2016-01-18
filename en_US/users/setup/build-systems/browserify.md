# Browserify

### Installation

```sh
$ npm install --save-dev babelify
```

### Usage

#### Via CLI

```sh
$ browserify script.js -t babelify --outfile bundle.js
```

#### Via Node API

```js
browserify({ debug: true })
  .transform(babelify);
```

Or a more complete example:

```js
var fs = require("fs");
var browserify = require("browserify");
var babelify = require("babelify");

browserify({ debug: true })
  .transform(babelify)
  .require("./script.js", { entry: true })
  .bundle()
  .on("error", function (err) { console.log("Error: " + err.message); })
  .pipe(fs.createWriteStream("bundle.js"));
```

#### Passing options

##### CLI

```sh
$ browserify -d -e script.js -t [ babelify --blacklist regenerator ]
```

##### Node API

```js
browserify().transform(babelify.configure({
  blacklist: ["regenerator"]
}))
```

##### `package.json`

```js
{
  "transform": [["babelify", { "blacklist": ["regenerator"] }]]
}
```

> For more information see the
> [babel/babelify repo](https://github.com/babel/babelify).
