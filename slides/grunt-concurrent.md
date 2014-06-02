## grunt-concurrent

```js
concurrent:{
  sassBrowserify: [
    'sass:theme',
    'jshint:themejs',
    'browserify:themejs'
  ]
}
```

> Run grunt tasks concurrently.
