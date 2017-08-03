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
✔ example1 x 83,285 ops/sec ±0.83% (86 runs sampled)
```

### Glob of files
```console
$ benchmark ./test/*.js
✔ example1 x 84,518 ops/sec ±0.90% (87 runs sampled)
✔ example2 x 1,612,805 ops/sec ±1.81% (80 runs sampled)
```

### Evaluate script
```console
$ benchmark -e "for (var i = 1000; i--;);"
✔ eval-1 x 244,076 ops/sec ±1.17% (86 runs sampled)
```

### Evaluate multiple scripts
```console
$ benchmark -e "1 + 1" -e "1 + 2"
✔ eval-1 x 1,561,524 ops/sec ±2.24% (77 runs sampled)
✔ eval-2 x 1,633,941 ops/sec ±1.76% (82 runs sampled)
```

### Contributions

Please feel free to create a PR!
