### Your First Grunt Project ###

> Let's get that magic sauce!!

--

### How? ###

- Install Node.js <!-- .element: class="fragment" data-fragment-index="1" -->
- Define your project <!-- .element: class="fragment" data-fragment-index="2" -->
- Get the goods <!-- .element: class="fragment" data-fragment-index="3" -->
- Configure the tasks <!-- .element: class="fragment" data-fragment-index="4" -->
- Reap the benefits! <!-- .element: class="fragment" data-fragment-index="5" -->

--

### Node.JS ###

```shell
$ brew install node
```

_or_ Download the [binary installer](http://nodejs.com)


--

### `Package.json` ###

- Like the module.info file, but for NPM
- Node Package Management delivers the tools

note:

- Format that node.js and NPM want
- Lists the dependencies
  - Similar to a module
  - Adds functionality to the base system

--

### Use the CLI Utility

```sh

$ cd my-awesome-theme
$ npm init

This utility will walk you through creating a package.json file.
It only covers the most common items, and tries to guess sane defaults.
...
Press ^C at any time to quit.
name: (my-awesome-theme)

```

note:
Nice utility to build the package.json

--

### What is this look like

Simplest version.
```json
{
  "name": "My Aweomse Theme!",
  "version": "0.1.0"
}
```

--

### Grunt CLI

```shell
$ npm install grunt-cli -g
```
> `-g` Makes grunt CLI Global!

--

### Install a task

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

--

### Package.json ###

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

--

### `Gruntfile.js` ###

```js
module.exports = function(grunt){});
```
--

### Begin

```js
module.exports = (grunt) ->
  'use strict'
  grunt.initConfig({
    package: grunt.file.readJSON 'package.json'

  })
```
