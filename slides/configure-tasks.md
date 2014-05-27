## Configure Tasks

```js
// 1. Use grunt and expose this functionality
module.exports = function(grunt){
  // 2. `initConfig` method to configure tasks.
  grunt.initConfig({
    package: grunt.file.readJSON('package.json')
  });
};
```
note:


--

### SASS Task

```js
module.exports = function(grunt){
  grunt.initConfig({
    package: grunt.file.readJSON('package.json'),
    // task
    sass: {
      // target
      theme:
        // files
        files: {
          'dist/scss/main.css' : 'scss/main.scss'
        }
    }
  });
};
```


--

### Load NPM Task

```js
// Make the plugin accessible to grunt.
grunt.loadNpmTasks('grunt-contrib-sass');
```


--

### Default Task

Runs with `$ grunt`

```js
grunt.registerTask(
  'default',
  'Compile SASS',
  ['sass:theme']
);
```
