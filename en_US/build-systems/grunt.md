### Installation

```sh
$ npm install --save-dev grunt-babel
```

### Usage

```js
require("load-grunt-tasks")(grunt); // npm install --save-dev load-grunt-tasks

grunt.initConfig({
  "babel": {
    options: {
      sourceMap: true
    },
    dist: {
      files: {
        "dist/app.js": "src/app.js"
      }
    }
  }
});

grunt.registerTask("default", ["babel"]);
```

> For more information see the
> [babel/grunt-babel repo](https://github.com/babel/grunt-babel).
