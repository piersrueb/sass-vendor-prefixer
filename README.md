### Sass Vendor Prefixer

Usage:

```scss
.my-class {
    @include prefixer("transition", "background-color 0.2s, height 0.4s");
}
```

Result:

```css
.my-class {
    -moz-transition: background-color 0.2s, height 0.4s;
    -ms-transition: background-color 0.2s, height 0.4s;
    -o-transition: background-color 0.2s, height 0.4s;
    -webkit-transition: background-color 0.2s, height 0.4s;
    transition: background-color 0.2s, height 0.4s;
}
```
