### Installation

```sh
$ npm install --save-dev babel-register
```

### Usage

Wherever you are calling Mocha add the following options:

```diff
- mocha
+ mocha --compilers js:babel-register"
```
