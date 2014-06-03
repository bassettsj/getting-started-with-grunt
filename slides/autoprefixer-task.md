##  Autoprefixer Task

![screenshot of the google search results for grunt autoprefixer](img/google-grunt-autoprefixer.png)


--

### Grunt Plugin Directory

![Table showing gruntplugins with a description](img/grunt-plugin-directory.png)

[gruntjs.com/plugins](http://gruntjs.com/plugins)

--

### Check the docs, look for the example


> README.md

```js
grunt.initConfig({

  autoprefixer: {

    options: {
      // Task-specific options go here.
    },

    // prefix the specified file
    single_file: {
      options: {
        // Target-specific options go here.
      },
      src: 'src/css/file.css',
      dest: 'dest/css/file.css'
    },

    // prefix all files
    multiple_files: {
      expand: true,
      flatten: true,
      src: 'src/css/*.css', // -> src/css/file1.css, src/css/file2.css
      dest: 'dest/css/' // -> dest/css/file1.css, dest/css/file2.css
    },

    // if you have specified only the `src` param, the destination will be set automatically,
    // so source files will be overwritten
    no_dest: {
      src: 'dest/css/file.css' // globbing is also possible here
    },

    diff: {
        options: {
            diff: true
        },
        src: 'src/css/file.css',
        dest: 'dest/css/file.css' // -> dest/css/file.css, dest/css/file.css.patch
    },

    sourcemap: {
        options: {
            map: true
        },
        src: 'src/css/file.css',
        dest: 'dest/css/file.css' // -> dest/css/file.css, dest/css/file.css.map
    },
  }

});

```

note:

Finding the Grunt plugin you want to use, I always quickly scroll to the examples and get roughly the task you need.

--

### Install, load, configure


1. `npm install -D grunt-autoprefixer`
2. configure task from the example

```js
...
autoprefixer: {
  theme: {
    options: {
      map: true
    },
    src: 'dist/css/**/*.css' // can leave the dest off
  }
}
```

--

### Install, load, configure

- `grunt.loadNpmTask('grunt-autoprefixer');`
- Add to the default task
- `$ grunt` compiled and prefixed -- oooh!

```js
grunt.registerTask(
  'default',
  'Compile SASS and autoprefix',
  [
    'sass:theme',
    'autoprefixer:theme'
  ]
);
```


<span class="fa fa-money fa-badge" aria-hidden="true"></span>
