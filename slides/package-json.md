## `Package.json` ###

- Like the module.info file, but for NPM
- Node Package Management delivers the tools

note:

- Format that node.js and NPM want
- Lists the dependencies
  - Similar to a module
  - Adds functionality to the base system

--

### package.json

```json
{
  "name": "awesome_theme",
  "version": "0.0.0",
  "description": "An awesome drupal theme",
  "main": "src/index.js",
  "scripts": {
    "test": "grunt test"
  },
  "keywords": [
    "Drupal",
    "theme",
    "grunt"
  ],
  "author": "Steven Bassett <steven.j.bassett@gmail.com>",
  "license": "BSD-2"
}
```


--

### `npm init` CLI Utility

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
