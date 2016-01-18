### Installation

```sh
$ npm install --save-dev babel-core
```

### Usage

In your `spec/support/jasmine.json` file make the following changes:

```js
{
  "helpers": [
    "../../node_modules/babel-register/lib/node.js"
  ]
}
```

This file is created when you setup a project with the `jasmine init` command.

> For more information see the
> [piecioshka/test-jasmine-babel repo](https://github.com/piecioshka/test-jasmine-babel).
