### Installation

```sh
$ npm install --save-dev duo-babel
```

### Usage

#### Via CLI

```sh
$ duo --use duo-babel
```

#### Via Node API

```js
Duo(root)
  .entry(entry)
  .use(babel)
  .run(fn);
```

> For more information see the
> [babel/duo-babel repo](https://github.com/babel/duo-babel).
