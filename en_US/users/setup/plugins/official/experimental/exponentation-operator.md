# Exponentation Operator

## Example

**Input**

```js
2 ** 2;
```

**Output**

```js
Math.pow(2, 2);
```

> Note that the output may not be exactly what is above. Babel's implementation
> may have changed since this document was last updated, or the output may have
> been cleaned up for clarity.

## Setup

### Installation

```sh
$ npm install --save-dev babel-plugin-transform-exponentation-operator
```

### Usage

#### Via `.babelrc` (recommended)

**`.babelrc`**

```json
{
  "plugins": ["transform-exponentation-operator"]
}
```

#### Via CLI

```sh
babel script.js --plugin transform-exponentation-operator
```

#### Via Node API

```js
require("babel-core").transform("code", {
  plugins: ["transform-exponentation-operator"]
});
```
