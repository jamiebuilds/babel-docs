### Installation

```sh
$ npm install --save-dev babel-brunch
```

### Usage

That's it! Set babel options in your brunch config (such as
`brunch-config.coffee`) except for filename and sourceMap which are handled
internally.

```yaml
plugins:
  babel:
    whitelist: ["arrowFunctions"]
    format:
      semicolons: false
```

> For more information see the
> [babel/babel-brunch repo](https://github.com/babel/babel-brunch).
