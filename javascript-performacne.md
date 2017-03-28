# JavaScript Performance

Speaker: @chancancode

Opened up with 10 minutes of jokes, not related to the talk thus far.

## Hierarchy of speed

1. Las of physics
1. hardware
1. kernals
1. userland
1. human factor


## Hierarchy of JavaScript performance

1. JS engined
1. Libraries
1. Your code

 Budget -> you get about 1,000 ms

## Your Code

### Micro vs Macro

* **Macro**: do fewer things
* **Micro**: do things faster

### Hidden loops

* Big data -- lots of data -- can lead to slow rendering (obviously)
* Backtracking -- invalidating already flushed content

### Micro vs Macro working

* Macro work
  * don't do the work work
  * Reuse work
  * defer the work
* Micro work
  * Use helpers
  * `{{unbound}}`
  * Custom components

## Tools

* Network tab
* Ember debugger
* Timeline view from chrome debugger
* `User Timing API` can be used to see what's happening when doing work in the JS
* `ember-bench`
* lighthouse
* pwmetrics

## Libraries

* Kind of do the work, you don't have to worry as much here in what you use. e.g. `Ember.get('')`

## JS Engines

* Modern eninges are faster now than they used to be
* They use a "hidden class" that keeps track of the objects
