# Make

### Installation

Installed already on *most* Unix systems. Available from
[gow](https://github.com/bmatzelle/gow) on Windows.

### Usage

```make
SRC = $(wildcard src/*.js)
LIB = $(SRC:src/%.js=lib/%.js)

lib: $(LIB)
lib/%.js: src/%.js
  mkdir -p $(@D)
  babel $< -o $@
$ make
```

```sh
$ make
```
