## PHP tools

- [grunt-phpcs](https://github.com/SaschaGalley/grunt-phpcs)
- [grunt-phplint](https://github.com/jgable/grunt-phplint)
- [grunt-phpunit](https://github.com/SaschaGalley/grunt-phpunit)
- [grunt-drush](https://github.com/nickpack/grunt-drush)


--

### PHP CodeSniffer

```js
phpcs: {
  theme: {
    // Let's sniff out template.php for Drupal coding standards.
    dir: ['template.php'],
    // Configure where to find it and what standard.
    options: {
      bin: './vendor/bin/phpcs',
      standard: 'Drupal'
    }
  }
}
```

--

### PHP Lint

```
$ grunt phplint
Running "phplint:template" (phplint) task
Warning:
Parse error: parse error, expecting `'{'' in template.php on line 10
Errors parsing template.php Use --force to continue.

Aborted due to warnings.
```


--

### PHP Unit

```js
phpunit: {
  classes: {
    // load the test classes from here.
    dir: 'tests/php/'
  },
  options: {
    // Pull from composer folder.
    bin: 'vendor/bin/phpunit',
    // The bootstrap file to get the test going.
    bootstrap: 'tests/php/phpunit.php',
    colors: true
  }
}

```

note:




--

### Drush


```js
drush: {
  // Turn off css and js preprocessing.
  disjscss:{
    args: ['vset preprocess 0']
  },
  // Turn on css and js preprocessing.
  enjscss:{
    args: ['vset preprocess 1']
  },
  // Clear the theme registry, could add as a watch task!
  ccthemereg:{
    args: ['cc theme-registry']
  },
  // Enable devel themer quickly.
  enthemer:{
    args: ['en devel_themer simplehtmldom -y']
  },
  // Disable devel themer quickly.
  disthemer:{
    args: ['dis devel_themer simplehtmldom -y']
  }
}
```
