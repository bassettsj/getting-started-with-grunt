## What about Gulp?

![Gulp Logo](img/gulp.png)

> Fear of using the wrong tool!<!-- .element: class="fragment" data-index="0" -->

Many of the same principles carry over, and Grunt isn't dead. <!-- .element: class="fragment" data-index="1" -->


--

### Gulp example

```
var gulp = require('gulp');
var sass = require('gulp-sass');

// Here's a simple
gulp.task('build', function(){
  gulp.src('public/stylesheets/scss/*.scss')
    .pipe(sass())
    .pipe(gulp.dest('dist/css/'));
});

```
