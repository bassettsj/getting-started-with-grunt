##  JShint Task

```js
jshint: {
  options: {
    jshintrc: true,
    reporter: require('jshint-stylish')
  },
  grunt:{
    files: { src: 'Gruntfile.js'}
  },
  themejs: {
    files: {
      src: 'src/**/*.js'
    }
  }
}
```
