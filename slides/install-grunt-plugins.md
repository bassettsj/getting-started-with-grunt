## Install Grunt Plugins

- grunt-contrib-uglify
- grunt-contrib-jshint
- grunt-contrib-qunit
- grunt-contrib-watch

[Grunt Plugins: gruntjs.com/plguins](http://gruntjs.com/plguins)

note:

Contrib means it is maintianed by the core grunt team.

But there are a plenty to checkout.

--

### Use npm to install local grunt

```shell
npm install --save-dev grunt

```

note:

Protip:
`-D` flag for saving to save for


--

### Updated package.json

```json
{
  "name": "Aweomse Theme!",
  "version": "0.0.0",
  ...
  "devDependencies": {
    "grunt": "~0.4.5"
  }
}
```
