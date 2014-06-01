##  load-grunt-config

You should probably do this!

```js
//Gruntfile.js
module.exports = function(grunt){
  'strict'
  require("load-grunt-config")(grunt);
};

//grunt/sass.js
module.exports = {
  // target
  theme:{
    options:{
      // note* requires SASS >=3.3.0 `gem install sass --pre`
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
