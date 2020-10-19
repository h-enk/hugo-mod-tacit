> __Tacit__ is a primitive CSS framework for dummies, like myself, who don't know anything about graphic design but want their web services to look eatable. No classes, no layouts. Just design plain and simple web pages compliant with HTML5 and they will look OK.

See: https://github.com/yegor256/tacit

## Use

Import the module into your Hugo project's site config:

```toml
[[module.imports]]
path = "github.com/h-enk/hugo-mod-tacit"
```

The styles gets mounted in `assets/scss/vendor/tacit`.

This means that they can be used like this in a Hugo template:

```html
{{ $scss := resources.Get "scss/vendor/tacit/main.scss" }}
{{ $style := $scss | resources.ToCSS }}
```
