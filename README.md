[![NPM version](https://badge.fury.io/js/%40dizmo%2Ffunctions-viewer.svg)](https://npmjs.org/package/@dizmo/functions-viewer)
[![Build Status](https://travis-ci.com/dizmo/functions-viewer.svg?branch=master)](https://travis-ci.com/dizmo/functions-viewer)
[![Coverage Status](https://coveralls.io/repos/github/dizmo/functions-viewer/badge.svg?branch=master)](https://coveralls.io/github/dizmo/functions-viewer?branch=master)

# @dizmo/functions-viewer

Module.

## Usage

### Installation

```sh
npm install @dizmo/functions-viewer --save
```

### Import

```javascript
import '@dizmo/functions-viewer';
```

### Example(s)

```javascript
...
```

## Development

### Clean

```sh
npm run clean
```

### Build

```sh
npm run build
```

#### without linting and cleaning:

```sh
npm run -- build --no-lint --no-clean
```

#### with UMD bundling (incl. minimization):

```sh
npm run -- build --prepack
```

#### with UMD bundling (excl. minimization):

```sh
npm run -- build --prepack --no-minify
```

### Lint

```sh
npm run lint
```

#### with auto-fixing:

```sh
npm run -- lint --fix
```

### Test

```sh
npm run test
```

#### without linting, cleaning and (re-)building:

```sh
npm run -- test --no-lint --no-clean --no-build
```

### Cover

```sh
npm run cover
```

#### without linting, cleaning and (re-)building:

```sh
npm run -- cover --no-lint --no-clean --no-build
```

## Debugging

Connect `@dizmo/functions-viewer` to another project:

```sh
[@dizmo/functions-viewer] $ npm link # symlink global:@dizmo/functions-viewer
```

```sh
[a-project] $ npm link @dizmo/functions-viewer # symlink node-modules:@dizmo/functions-viewer
```

```sh
[a-project] $ head webpack.config.js # ensure @dizmo/functions-viewer in entry.main
```

```
entry: {
    main: [..., '@dizmo/functions-viewer', './source/index.js']
}
```

Disconnect `@dizmo/functions-viewer` from the project:

```sh
[a-project] $ npm unlink @dizmo/functions-viewer # delete local symlink
```

```sh
[@dizmo/functions-viewer] $ npm uninstall -g # delete global symlink
```

## Documentation

```sh
npm run docs
```

## Publication

```sh
npm publish
```

#### initially (if public):

```sh
npm publish --access=public
```

## Copyright

 © 2021 [Hasan Karahan](https://github.com/hsk81)
