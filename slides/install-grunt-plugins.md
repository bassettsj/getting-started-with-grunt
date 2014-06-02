## Install Grunt Plugins

Take a look at Grunt website for a great index of popular plugins.

- grunt-contrib-uglify
- grunt-contrib-jshint
- grunt-contrib-qunit
- grunt-contrib-watch
- .... so many! <!-- .element: class="fragment" data-index="0" -->

note:



--

### Use npm to install local grunt

```shell
npm install --save-dev grunt

```
#### Protip:
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
