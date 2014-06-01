##  But wait...

This is no different than just running...

```sh
$ sass scss/main.scss css/main.css
```

--

### The power comes from multiple tasks.

so lets add some more


--

### Autoprefixer

```css

:fullscreen a {
    transition: transform 1s
}

/* becomes */
:-webkit-full-screen a {
    -webkit-transition: -webkit-transform 1s;
    transition: transform 1s
}
:-moz-full-screen a {
    transition: transform 1s
}
:-ms-fullscreen a {
    transition: transform 1s
}
:fullscreen a {
    -webkit-transition: -webkit-transform 1s;
    transition: transform 1s
}

```

and there is a grunt task for that!<!-- .element class="fragment" data-index="0" -->
