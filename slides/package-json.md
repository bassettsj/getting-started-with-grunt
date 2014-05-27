## `Package.json` ###

- Like the module.info file, but for NPM
- Node Package Management delivers the tools

note:

- Format that node.js and NPM want
- Lists the dependencies
  - Similar to a module
  - Adds functionality to the base system

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

--

### What is this look like

Simplest version.
```json
{
  "name": "My Aweomse Theme!",
  "version": "0.1.0"
}
```
