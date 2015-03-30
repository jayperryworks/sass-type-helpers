# Sass type helpers

Helper mixins for dealing with typography.

## Font scale

A simple modular scale mixin. Instead of strictly calculating a scale, this uses an array (or "list" in Sassinese) that you can modify.

````
// modular scale
$font-scale: 13px 16px 19px 26px 30px 42px 48px 68px 78px 110px;

h1 {
  @include font-scale(5);
  // outputs:
  // font-size: 30px;
  // font-size: 1.875rem;
}
````

## Headers selector

A helper function that selects a range of header tags.

````
#{headers(1,4)} { color: red; }

// outputs:
// h1, h2, h3, h4 { color: red; }
````
