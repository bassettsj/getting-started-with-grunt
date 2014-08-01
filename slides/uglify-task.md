##  Uglify Task

```js
uglify: {
  themejs: {
    options:{
      sourceMap: true, // Source maps for debugging issues.
      // A banner for the file itself, can pass a variable into the template.
      banner: '<%= banner %>'
    },
    // You can pass in other target config into the template function.
    src: '<%= browserify.themejs.dest  %>',
    dest: './dist/js/',
    ext: '.pkg.min.js',
  }
}
```
