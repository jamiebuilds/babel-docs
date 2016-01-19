# Merge Sibling Variables

Merge sibling variables declarations into one declaration.

## Example

**Input**

```js
var foo = "bar";
var bar = "foo";
```

**Output**

```js
var foo = "bar",
    bar = "foo";
```

> Note that the output may not be exactly what is above. Babel's implementation
> may have changed since this document was last updated, or the output may have
> been cleaned up for clarity.

## Setup

### Installation

```sh
$ npm install --save-dev babel-plugin-transform-merge-sibling-variables
```

### Usage

#### Via `.babelrc` (recommended)

**`.babelrc`**

```json
{
  "plugins": ["transform-merge-sibling-variables"]
}
```

#### Via CLI

```sh
babel script.js --plugin transform-merge-sibling-variables
```

#### Via Node API

```js
require("babel-core").transform("code", {
  plugins: ["transform-merge-sibling-variables"]
});
```
