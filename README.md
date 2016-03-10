> Official Podio JavaScript SDK for Node and the browser

## Installation

```sh
$ npm install podio-js --save
```

## Usage

#### Node

```js
var Podio = require('podio-js').api;

var podio = new Podio({
  authType: 'server',
  clientId: 'id',
  clientSecret: 'secret'
});
```

#### Express Middleware

Simple express middleware for storing the Podio token

```js
app.use(require('podio-js').middleware({
  clientId: 'id',
  clientSecret: 'secret'
}));
```

#### Browser

If you are using and AMD/CommonJS compatible module loader you can require the module:

```js
var PodioJS = require('podio-js');
```

If you are not using a loader, browserify `podio-js` like this:

```sh
$ npm install -g browserify

$ npm run bundle
```

and include `dist/podio-js.js` using a `<script>` tag.

## Documentation

You will find a detailed documentation at [http://podio.github.io/podio-js/](http://podio.github.io/podio-js/) and at [https://developers.podio.com/](https://developers.podio.com/)


## Tests

```sh
$ npm test
```
