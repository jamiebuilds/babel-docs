### Installation

```sh
$ npm install --save-dev gulp-babel
```

### Usage

```js
var gulp = require("gulp");
var babel = require("gulp-babel");

gulp.task("default", function () {
  return gulp.src("src/app.js")
    .pipe(babel())
    .pipe(gulp.dest("dist"));
});
```

Use [gulp-sourcemaps](https://github.com/floridoo/gulp-sourcemaps) like this:

```js
var gulp = require("gulp");
var sourcemaps = require("gulp-sourcemaps");
var babel = require("gulp-babel");
var concat = require("gulp-concat");

gulp.task("default", function () {
  return gulp.src("src/**/*.js")
    .pipe(sourcemaps.init())
    .pipe(babel())
    .pipe(concat("all.js"))
    .pipe(sourcemaps.write("."))
    .pipe(gulp.dest("dist"));
});
```

> For more information see the
> [babel/gulp-babel repo](https://github.com/babel/gulp-babel).
