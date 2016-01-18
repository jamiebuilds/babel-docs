# ES2015 Template Literals

Compile ES2015 template literals to ES5

## Example

**Input**

```js
`test ${value}`;
```

**Output**

```js
"test " + value;
```

> Note that the output may not be exactly what is above. Babel's implementation
> may have changed since this document was last updated, or the output may have
> been cleaned up for clarity.

## Setup

### Installation

```sh
$ npm install --save-dev babel-plugin-transform-es2015-template-literals
```

### Usage

#### Via `.babelrc` (recommended)

**`.babelrc`**

```json
{
  "plugins": ["transform-es2015-template-literals"]
}
```

#### Via CLI

```sh
babel script.js --plugin transform-es2015-template-literals
```

#### Via Node API

```js
require("babel-core").transform("code", {
  plugins: ["transform-es2015-template-literals"]
});
```
