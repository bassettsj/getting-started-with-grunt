##  CSSmin, JShint, browserify, uglifyjs...

<span class="fa fa-clock fa-4x" aria-hidden="true"></span>

For the sake of time...

```js
...
cssmin:{
  theme:{
    files: {
      expand: true,
      cwd: 'dist/css/'
      src: [
        '**/*.css',
        '!**/*.min.css'
      ],
      ext: '.min.css',
      dest: 'dist/css/'
    }
  }
}
```
<!-- element. class="fragment" data-index="0" -->

note:

To save time I am going to get some other tasks done quickly.


--

### JShint

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


}
