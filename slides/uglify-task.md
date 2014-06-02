##  Uglify Task

```js
uglify: {
  themejs: {
    options:{
      sourceMap: true,
      banner: '<%= banner %>'
    },
    src: '<%= browserify.themejs.dest  %>',
    dest: './dist/js/',
    ext: '.pkg.min.js',
    expand: true,
    flatten: true
  }
}
```
