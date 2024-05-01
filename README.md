# [jslib-base](https://github.com/yanhaijing/jslib-base)

[![](https://img.shields.io/badge/Powered%20by-jslib%20base-brightgreen.svg)](https://github.com/yanhaijing/jslib-base)
[![license](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/yanhaijing/jslib-base/blob/master/LICENSE)
[![npm](https://img.shields.io/badge/npm-3.0.6-orange.svg)](https://www.npmjs.com/package/@js-lib/cli)
[![NPM downloads](http://img.shields.io/npm/dm/@js-lib/cli.svg?style=flat-square)](http://www.npmtrends.com/@js-lib/cli)
[![Percentage of issues still open](http://isitmaintained.com/badge/open/yanhaijing/jslib-base.svg)](http://isitmaintained.com/project/yanhaijing/jslib-base 'Percentage of issues still open')
![example workflow](https://github.com/yanhaijing/jslib-base/actions/workflows/ci.yml/badge.svg)

English | [简体中文](https://github.com/yanhaijing/jslib-base/blob/master/README.zh-CN.md)

The best `JS|TS` third-party library scaffold, quickly setup the basic framework of a `JS|TS` library in 10 seconds.

**Libraries based on jslib-base can be shared on the [jsmini](https://github.com/jsmini) platform.**

## :star: Features

- **Interactive CLI for project initialization**
- **Upgrade functionality** – Easily upgrade old libraries with one command
- **Supports both JavaScript and TypeScript**
- **Build & Packaging Solutions**
  - TypeScript + Babel + Rollup
  - Automatic third-party dependency injection (supports tree shaking)
- **Multi-Environment Compatibility**
  - Supports native browser script usage
  - Provides UMD and ESM modules, compatible with Webpack, Vite, and other ecosystems
  - Adapts to both old and new Node.js module systems (CommonJS + ESM)
- **Code Style & Linting**
  - ESLint + Prettier + Husky + Lint-Staged
- **Unit Testing Suite**
  - Mocha + Expect.js + Istanbul + NYC + Coveralls
- **Commit Linting**
  - Commitlint + Commitizen
- **GitHub Actions**
  - CI + Release
- **Local Development Server**
  - http-server

## :rocket: User Guide

To create a new project, it is recommended to use Node.js version 18 or higher.

```bash
$ npx @js-lib/cli new mylib
# Interactive queries, input project info
$ cd mylib
$ npm i
```

To update the project, just execute the following command in the project root directory.

```bash
$ npx @js-lib/cli update
```

For old projects, you can't directly execute the update command, you can first initialize a config file.

```bash
$ npx @js-lib/cli new -c
```

Directory Overview

```
.
├── demo Usage demo
├── dist Compiled out code
├── doc Project documents
├── src Source code directory
├── test Unit tests
├── CHANGELOG.md Change log
└── TODO.md To-do features
```

Common command scripts

```bash
$ npm run lint
$ npm run test
$ npm run build
$ npm run release
$ npm publish
```

## Contribution Guide

If you only want to modify the library code generated by the CLI, you can directly edit the template code, which is simpler.

After merging, I will migrate the template to the CLI. The template repository is as follows:

- [jslib](https://github.com/yanhaijing/jslib)
- [tslib](https://github.com/yanhaijing/tslib)

This project uses lerna to manage multiple plugins, common lerna commands are:

```bash
$ npx lerna init # Initialization
$ npx lerna create @js-lib/todo # Create a package
$ npx lerna add yargs --scope=@js-lib/cli # Install dependencies for a package
$ npx lerna list # List all the packages
$ npx lerna bootstrap # Install all dependencies
$ npx lerna link # Create all links
$ npx lerna changed # List the packages to be updated in the next release
$ npx lerna publish # Release with tag, upload to git, upload to npm
```

## Contributors

[contributors](https://github.com/yanhaijing/jslib-base/graphs/contributors)

## Change Log

[CHANGELOG.md](https://github.com/yanhaijing/jslib-base/blob/master/CHANGELOG.md)

## TODO

[TODO.md](https://github.com/yanhaijing/jslib-base/blob/master/TODO.md)

## Current Users

- [jsmini](https://github.com/jsmini)
- [template.js](https://github.com/yanhaijing/template.js)
- [shin-monitor](https://github.com/pwstrick/shin-monitor)
- [baselib](https://github.com/LesixCoder/utils)
- [streaming-json-js](https://github.com/karminski/streaming-json-js)
- [better-js-lib](https://github.com/SFTC/better-js-lib)
- [...](https://github.com/yanhaijing/jslib-base/issues/10)
