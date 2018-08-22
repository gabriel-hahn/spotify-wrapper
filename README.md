# spotify-clone-javascript-tdd

[![Build Status](https://travis-ci.org/gabriel-hahn/spotify-clone-javascript-tdd.svg?branch=master)](https://travis-ci.org/gabriel-hahn/spotify-clone-javascript-tdd)

[![Coverage Status](https://coveralls.io/repos/github/gabriel-hahn/spotify-clone-javascript-tdd/badge.svg?branch=master)](https://coveralls.io/github/gabriel-hahn/spotify-clone-javascript-tdd?branch=master)

A Spotify player clone with a wrapper to work with the follow API:

[Spotify Web API](https://developer.spotify.com/documentation/web-api/)

[Airbnb Style Guide](https://github.com/airbnb/javascript)

# Browser Support

This library relies on [Fetch API](https://fetch.spec.whatwg.org/). And this project is supported in the following browsers:

![Chrome](https://cloud.githubusercontent.com/assets/398893/3528328/23bc7bc4-078e-11e4-8752-ba2809bf5cce.png) | ![Firefox](https://cloud.githubusercontent.com/assets/398893/3528329/26283ab0-078e-11e4-84d4-db2cf1009953.png) | ![Opera](https://cloud.githubusercontent.com/assets/398893/3528330/27ec9fa8-078e-11e4-95cb-709fd11dac16.png) | ![Safari](https://cloud.githubusercontent.com/assets/398893/3528331/29df8618-078e-11e4-8e3e-ed8ac738693f.png) | ![IE](https://cloud.githubusercontent.com/assets/398893/3528325/20373e76-078e-11e4-8e3a-1cb86cf506f0.png) |
--- | --- | --- | --- | --- |
39+ | 42+ | 29+ | 10.1+ | Nope |

# Dependencies

This library depends on [fetch](https://fetch.spec.whatwg.org/) to make requests to the Spotify Web API. For environments that don't support fetch, you'll need to provide a [polyfill](https://github.com/github/fetch) to browser or [polyfill](https://github.com/bitinn/node-fetch) to Node.

# Installation

```sh
$ npm install spotify-wrapper --save
```

# How to use

### ES6

```js
// To import a specific method
import { method } from 'spotify-wrapper';

// To import everything
import * as spotifyWrapper from 'spotify-wrapper';
```

### CommonJS

```js
var spotifyWrapper = require('spotify-wrapper');
```

### UMD in Browser

```html
<!-- To import non-minified version -->
<script src="spotify-wrapper.umd.js"></script>

<!-- To import minified version -->
<script src="spotify-wrapper.umd.min.js"></script>
```

After that the library will be available to the Global as `spotifyWrapper`.
Follow as example:

```js
const albums = spotifyWrapper.search.albums('Choosen Artist');
```
