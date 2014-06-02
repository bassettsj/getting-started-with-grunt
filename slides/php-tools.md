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
    dir: ['template.php'],
    options: {
      bin: './vendor/bin/phpcs',
      standard: 'Drupal'
    }
  }
},
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

### PHPunit

```js
phpunit: {
    classes: {
        dir: 'tests/php/'
    },
    options: {
        bin: 'vendor/bin/phpunit',
        bootstrap: 'tests/php/phpunit.php',
        colors: true
    }
}

```


--

### Drush


```js
drush: {
  disjscss:{
    args: ['vset preprocess 0']
  },
  enjscss:{
    args: ['vset preprocess 1']
  },
  ccthemereg:{
    args: ['cc theme-registry']
  },
  enthemer:{
    args: ['en devel_themer simplehtmldom -y']
  },
  disthemer:{
    args: ['dis devel_themer simplehtmldom -y']
  }
}
```
