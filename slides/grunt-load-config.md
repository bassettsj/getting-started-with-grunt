##  load-grunt-config

```js
//Gruntfile.js
module.exports = function(grunt){
  'strict'
  require("load-grunt-config")(grunt);
};
```
```js
//grunt/sass.js
// This is now where all your task config lives, in small digestable files.
module.exports = {
  // target
  theme:{
    options:{
      sourcemap: true
    },
    // files
    files: [{
      dest: 'dist/css/awesome-theme.css'
      src: 'scss/main.scss'
    }]
  }
}

```

note:
You should probably do this!



--

### Works with YML, CoffeeScript and JS too!

```yml
dafault:
  sass
  autoprefixer
  cssmin
  jshint
  browserify
  uglify
devel:
  clean:dist
  watch
```
