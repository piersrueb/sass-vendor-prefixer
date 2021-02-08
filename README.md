### Sass Vendor Prefixer

Sass mixin for adding vendor prefixes for broader support for newer properties in older browsers. Add and remove prefixes from the array within the mixin to suit your needs.

```scss
$prefixes: "moz", "ms", "o", "webkit";
```

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
