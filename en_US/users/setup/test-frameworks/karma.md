# Karma

### Installation

```sh
$ npm install --save-dev karma-babel-preprocessor
```

### Usage

```js
module.exports = function(config) {
  config.set({
    files: [
      "src/**/*.js",
      "test/**/*.js"
    ],
    preprocessors: {
      "src/**/*.js": ["babel"],
      "test/**/*.js": ["babel"]
    },
    "babelPreprocessor": {
      // options go here
    }
  });
};
```

> For more information see the
> [babel/karma-babel-preprocessor repo](https://github.com/babel/karma-babel-preprocessor).
