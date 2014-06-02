##  CSSmin Task

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

note:

To save time I am going to get some other tasks done quickly.
