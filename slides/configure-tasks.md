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

### Install SASS Task

`$ npm install --save-dev grunt-contrib-sass`

```json
{
  "name": "Aweomse Theme!",
  "version": "0.0.0",
  ...
  "devDependencies": {
    "grunt": "~0.4.5",
    "grunt-contrib-sass": "0.7.3"
  }
}
```

--

### SASS Task

```js
module.exports = function(grunt){
  grunt.initConfig({
    package: grunt.file.readJSON('package.json'),
    // task
    sass: {
      // target
      theme: {
        //Options
        options: {
          // note* requires SASS >=3.3.0 `gem install sass --pre`
          sourcemap: true,
          loadPath: [
            'bower_components',
            '...'
          ]
        },
        // files
        files: [{
          dest: 'dist/css/awesome-theme.css',
          src: 'scss/main.scss'

        }]
      }
    }
  });
};

```

note:

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
