# Bits.sass utilities: responsive dimension

Responsive superset of space utilities.

See [Bits.sass utils-dimension](https://github.com/bits-sass/utils-dimension)
for more about original utilities.

Read more about [Bits.sass toolkit](https://github.com/bits-sass/bits.sass).

## Installation

* __Bower:__ `bower install --save bits-sass-responsive-utils-dimension`
* __Download:__ [zip](https://github.com/bits-sass/responsive-utils-dimension/zipball/master), [tar.gz](https://github.com/bits-sass/responsive-utils-dimension/tarball/master)
* __Git:__ `git clone https://github.com/bits-sass/responsive-utils-dimension.git`

## Available SASS variables

* `bits-utils-ns` - utilities namespace, defaults to 'bits-'
* `bits-responsive-dimension-columns` - list of column variations,
   used by `v[n]-u-sizeXofY`

## Available utility classes

* `v[n]-u-sizeFull` - make an element the width of its parent on `n` breakpoint
* `v[n]-u-sizeAuto` - shrink element's width to its natural value on `n`
breakpoint, should be used in conjunction with display utilities
* `v[n]-u-sizeXofY` (adjustable) - specifies the proportional width of an object
  on `n` breakpoint

## Usage

The `v[n]-u-size[Full|Auto]` utils can be used to widen an element on narrow
screens and then, on a wider screen, shrink it to its natural width.

```html
<button class="Button Button--primary u-sizeFull
               v4-u-sizeAuto v4-inlineBlock">Hit me!</button>
```

The `v[n]-u-sizeXofY` utils are especially useful in grid.

```html
<div class="Grid">
  <div class="Grid-cell u-size1of3 v4-u-size2of3">
    …
  </div>
  <div class="Grid-cell u-size2of3 v4-u-size1of3">
    …
  </div>
</div>
```

## Requirements

* Sass 3.2+

## Browser support

* Google Chrome (latest)
* Opera (latest)
* Firefox 4+
* Safari 5+
* Internet Explorer 9+ (IE 8 requires a build step)