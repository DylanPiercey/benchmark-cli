<h1 align="center">
  <!-- Logo -->
  <br/>
  benchmark-cli
	<br/>

  <!-- Stability -->
  <a href="https://nodejs.org/api/documentation.html#documentation_stability_index">
    <img src="https://img.shields.io/badge/stability-stable-brightgreen.svg?style=flat-square" alt="API stability"/>
  </a>
  <!-- Standard -->
  <a href="https://github.com/feross/standard">
    <img src="https://img.shields.io/badge/code%20style-standard-brightgreen.svg?style=flat-square" alt="Standard"/>
  </a>
  <!-- NPM version -->
  <a href="https://npmjs.org/package/benchmark-cli">
    <img src="https://img.shields.io/npm/v/benchmark-cli.svg?style=flat-square" alt="NPM version"/>
  </a>
  <!-- Downloads -->
  <a href="https://npmjs.org/package/benchmark-cli">
    <img src="https://img.shields.io/npm/dm/benchmark-cli.svg?style=flat-square" alt="Downloads"/>
  </a>
</h1>

Quickly run some benchmarks from the CLI.
Supports requiring dependencies and uses [benchmark.js](https://benchmarkjs.com) internally.

# Installation

```console
npm install benchmark-cli -g
```

# Examples

### Single file
```console
$ benchmark ./test/example1.js
✔ ./test/example1.js x 74,792 ops/sec ±2.63% (81 runs sampled)
```

### Glob of files
```console
$ benchmark ./test/*.js
✔ ./test/example1.js x 74,792 ops/sec ±2.63% (81 runs sampled)
✔ ./test/example2.js x 1,440,522 ops/sec ±2.76% (78 runs sampled)
```

### Evaluate directly
```console
$ benchmark -e "for (var i = 1000; i--;);"
✔ evaluate x 213,961 ops/sec ±0.75% (88 runs sampled)
```

### Contributions

Please feel free to create a PR!
