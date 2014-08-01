##  JShint Task

```js
jshint: {
  // These options are global.
  options: {
    jshintrc: true, // Look for the .jshint.json config in the project.
    reporter: require('jshint-stylish') // Use a nicer reporter.
  },
  // This is separate target to check just the gruntfile itself.
  grunt:{
    files: { src: 'Gruntfile.js'}
  },
  // This looks at all the JS in the theme.
  themejs: {
    files: {
      src: 'src/**/*.js'
    }
  }
}
```
