## Install Grunt Plugins

Take a look at Grunt website for a great index of popular plugins.

- grunt-contrib-uglify
- grunt-contrib-jshint
- grunt-contrib-qunit
- grunt-contrib-watch
- grunt-contrib-sass
- grunt-contrib-cssmin
- grunt-contrib-coffee

--

### Use npm to install local grunt and plugins ###

```shell
npm install --save-dev grunt grunt-contrib-sass
npm install -D grunt-contrib-watch
```
#### Protip:
`-D` flag for saving to save for


--

### Updated package.json

```json
{
  "name": "My Aweomse Theme!",
  "version": "0.1.0",
  "devDependencies": {
    "grunt": "~0.4.5",
    "grunt-contrib-sass": "0.7.3",
    "grunt-contrib-watch": "~0.6.1"
  }
}
```
