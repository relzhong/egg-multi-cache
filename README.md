# egg-multi-cache

[![NPM version][npm-image]][npm-url]
[![build status][travis-image]][travis-url]
[![Test coverage][codecov-image]][codecov-url]
[![David deps][david-image]][david-url]
[![Known Vulnerabilities][snyk-image]][snyk-url]
[![npm download][download-image]][download-url]

[npm-image]: https://img.shields.io/npm/v/egg-multi-cache.svg?style=flat-square
[npm-url]: https://npmjs.org/package/egg-multi-cache
[travis-image]: https://img.shields.io/travis/eggjs/egg-multi-cache.svg?style=flat-square
[travis-url]: https://travis-ci.org/eggjs/egg-multi-cache
[codecov-image]: https://img.shields.io/codecov/c/github/eggjs/egg-multi-cache.svg?style=flat-square
[codecov-url]: https://codecov.io/github/eggjs/egg-multi-cache?branch=master
[david-image]: https://img.shields.io/david/eggjs/egg-multi-cache.svg?style=flat-square
[david-url]: https://david-dm.org/eggjs/egg-multi-cache
[snyk-image]: https://snyk.io/test/npm/egg-multi-cache/badge.svg?style=flat-square
[snyk-url]: https://snyk.io/test/npm/egg-multi-cache
[download-image]: https://img.shields.io/npm/dm/egg-multi-cache.svg?style=flat-square
[download-url]: https://npmjs.org/package/egg-multi-cache

node-cache-manager features a built-in memory cache (using node-lru-cache), with the standard functions you'd expect in most caches:
`
set(key, val, {ttl: ttl}) // * see note below
wrap(key, function, {ttl: ttl}) 
get(key)
del(key)

// * Note that depending on the underlying store, you may be able to pass the
// ttl as the third param, like this:
set(key, val, ttl)
// ... or pass no ttl at all:
set(key, val)`


## Install

```bash
$ npm i egg-multi-cache --save
```

## Usage

```js
// {app_root}/config/plugin.js
exports.multiCache = {
  enable: true,
  package: 'egg-multi-cache',
};
```

## Configuration

```js
// {app_root}/config/config.default.js
exports.multiCache = {
};
```

see [config/config.default.js](config/config.default.js) for more detail.

## Example

<!-- example here -->

## Questions & Suggestions

Please open an issue [here](https://github.com/relzhong/egg-multi-cache/issues).

## License

[MIT](LICENSE)
