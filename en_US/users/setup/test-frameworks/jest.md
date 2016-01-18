# Jest

### Installation

```sh
$ npm install --save-dev babel-jest
```

### Usage

In your `package.json` file make the following changes:

```json
{
  "scripts": {
    "test": "jest"
  },
  "jest": {
    "scriptPreprocessor": "<rootDir>/node_modules/babel-jest",
    "testFileExtensions": ["es6", "js"],
    "moduleFileExtensions": ["js", "json", "es6"]
  }
}
```

> For more information see the
> [babel/babel-jest repo](https://github.com/babel/babel-jest).
