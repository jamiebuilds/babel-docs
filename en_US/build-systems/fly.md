### Installation

```sh
$ npm install -D fly-babel
```

### Usage

```js
export function* text() {
  yield this
    .source("src/**/*.js")
    .babel({ stage: 0 })
    .target("dist/")
}
```
