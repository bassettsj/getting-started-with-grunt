## Browserify Task


`$ npm install -D grunt-browserify browserify-shim`

```js
browserify: {
  themejs: {
    files:  {
      dest: 'dist/js/awesome-theme.pkg.js',
      src: 'src/index.js'
    }
  }
}
```

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
