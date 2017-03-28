# Opening Keynote

Speakers: Yehuda Katz, Tom Dale

Started a wee bit late. :-)

Overall this has been a history of Ember with some mentions of how Ember
has grown and what has changed overtime.


## Starter notes

* One track only for this conference.
* Ember has been around for 5 years
* Code of conduct is very important to the conference
* Amber.js was the original name
* Tomster is the mascot
* Seems we got on to Ember at just the right time. 2.0 seems pretty awesome, at least thus far
* LTS releases started in 2016 -- reached official maturity
* Hard to make long term changes because there are already a lot of users in the Emberjs community
* Should likey use fastboot for fast pages
* Ember Engines for small chunks of applications, may load faster
* ES2015 modules are supported out of the box
* Ember 2.x series has been very good at not causing breaks


## What did they learn?

* Big up front design -- didn't quite work, need more user feedback while developing
* Build small kernal of Ember and let Addons build better/more functionality
* Need to have drop-in replacements
* Experimentation has helped -- ember-redux, ember-concurrency, ember-orbit
* Experimentation has shown some busted bits -- liquid-fire, smoke-and-mirrors
* Pods didn't really work out, so now they are doing "Module Unification"
* Lean on small primitives and compatiblity

## Wins

* Wire frame style of the templates made it easier to optimize them at compile time

## Benchmarks

* They can be misleading, because they are not necessarily what you need to focus on
* Initial Render time on frameworks is a little slow for Glimmer
* Update is super fast for glimmer, basically the best one
* On realistic content Glimmer is almost the best, Inferno is the best still for initial render
* Update is way faster for Glimmer with real content
* Want initial render and update performance to be good, without having to think about it a lot for the application devleoper -- coolio

## Glimmer

* Glimmer has stuff for things for typescript
* Decoratoers can be used to help with computed properties
* With `@tracked` you can stop using `.get` and `.set`
* Glimmer helps make the size of stuff much smaller for apps
* `@` used in templates to show passed variables
* This is the desired Component API for Ember

## Other bits

* Module unification feature, is a desired state for improving module structure
* TypeScript will be supported, but not required
