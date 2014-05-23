### Your First Grunt Project ###

- SASS / LESS / CSS
  - Compiled
  - Linted
  - Prefixed
  - Minified
- Coffeescript / Javascript
  - Linted
  - Unit Tested
  - Concatinated
  - Minified

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

*or* Download the binary installer <!-- .element: class="fragment" data-fragment-index="1" -->


--

### `Package.json` ###

- Node Package Management delivers the tools
- `$ npm init`

```json
{
  "name": "My Aweomse Theme!",
  "version": "0.1.0"
}
```



--

### `Gruntfile.js` ###

```coffeescript
module.exports = (grunt) ->
  'use strict'
  grunt.initConfig({
    package: grunt.file.readJSON 'package.json'

  })
```
