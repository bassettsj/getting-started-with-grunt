## grunt-newer

```js
watch: {
  scss: {
    files: ['...']
    tasks: [
      'newer:sass:theme',
      // Will only run task on files that have changed,
      // since the last time the task
      'newer:autoprefixer:theme'
    ]
  }
}
```
