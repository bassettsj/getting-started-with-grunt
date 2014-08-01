## Browserify Task


`$ npm install -D grunt-browserify browserify-shim`

```js
browserify: {
  themejs: {
    files:  {
      dest: 'dist/js/awesome-theme.pkg.js', // The packaged modules ready to be used.
      src: 'src/index.js' // The browserify source index file to compile from.
    }
  }
}
```
Config within our package.json

```json
{
  "main": "src/index.js",
  "browserify-shim": {
    "jquery": "global:jQuery",
    "drupal": "global:Drupal"
  },
  "browserify": {
    "transform": [
      "browserify-shim"
    ]
  }
}
```
