# JSPM

### Installation

Select `babel` as the transpiler when running `jspm init -p` or to switch an
existing project into Babel use:

```sh
jspm dl-loader --babel
```

### Usage

Babel will automatically be used when loading any source with `import` or
`export` module syntax.

> JSX support is currently disabled by jspm. To re-enable it, add
> `"blacklist": []` to `babelOptions` in the jspm configuration file.
