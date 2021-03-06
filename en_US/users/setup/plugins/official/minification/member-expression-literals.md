# Member Expression Literals

Turn valid member expression property literals into plain identifiers

## Example

**Input**

```js
obj["foo"] = "isValid";
obj.const = "isKeyword";
obj["var"] = "isKeyword";
```

**Output**

```js
obj.foo = "isValid";
obj["const"] = "isKeyword";
obj["var"] = "isKeyword";
```

> Note that the output may not be exactly what is above. Babel's implementation
> may have changed since this document was last updated, or the output may have
> been cleaned up for clarity.

## Setup

### Installation

```sh
$ npm install --save-dev babel-plugin-transform-member-expression-literals
```

### Usage

#### Via `.babelrc` (recommended)

**`.babelrc`**

```json
{
  "plugins": ["transform-member-expression-literals"]
}
```

#### Via CLI

```sh
babel script.js --plugin transform-member-expression-literals
```

#### Via Node API

```js
require("babel-core").transform("code", {
  plugins: ["transform-member-expression-literals"]
});
```
