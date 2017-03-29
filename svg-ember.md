# SVG animation and interaction in Ember

Speaker: Jen Weber @jwwweber

UI/UX Developer at BioBright

So far talk is about SVG and SVG definitions.


## Objectives

* SVG Basics
* Using SVGs in Ember
* Avoiding pitfalls

## CSS Animations with SVGs

* Can use the CSS3 stuff
* Keyframes work
* Also the translation parts -- look at this site for SVG examples: https://sarasoueidan.com/

## Pitfalls

* top left is 0,0 (same as left, and top in CSS)
* `div` inside svg does not work, need to override the ember default
* need to look at paint order, so order data correctly for no bad overlays
* Need to be above Ember 1.8 (yay, that's the new default)

## General SVG Notes

* Some CSS attributes are different, e.g. `fill` and `stroke`
* no `z-index` it's all paint order
* use `g` for grouping
* Can use ember and it's action management on the `svg`
* `transform` can be used to easily change size/position of the svg
* Take a look at: https://sarasoueidan.com/blog/svgo-tools/

## Other libs

* ember-D3
* ember-highcharts
* ember-charts
