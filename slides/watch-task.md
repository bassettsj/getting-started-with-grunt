##  Watch Task

`$ npm install -D grunt-contrib-watch`

```js
...
watch:{
  sass: {
    files: 'scss',
    tasks: [
      'sass:theme',
      'autoprefixer:theme'
    ]
  }
}
...
grunt.loadNpmTasks('grunt-contrib-watch')
```

--

### Live Reload!?

No mo' refresh!

```js
watch:{
  sass: {...},
  livereload: {
    files: 'dist/**/*{.js|.css}', // Will only trigger reload once they are done being done.
    options: {
      livereload: true
    }
  }
```
