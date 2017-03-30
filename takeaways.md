# Takeaways

Below are some takeaways for me from Ember Conf 2017. They range from specifics during talks
to ideas that came up while talks where occuring. Mostly a quick bullet list of what to look into
and/or start using.

## Libraries to start using

* `ember-concurrency` -- this will help in areas where "is loading" or "waiting" is needed within the application.
* `ember-cli-content-security-policy` -- can help us with ensuring templates are a bit more secure in the usage of things like `_blank`

## Libraries to look into

* `liquid-fire` -- apparently everyone who is anyone uses this for animations
* `ember-service-worker` (add associated addons) -- can help with processing data on the frontend and for offline work with apps, will still need app cache
* `ember-power-select` -- should make dropdowns much easier
* `glimmer` -- may be good idea for small projects that don't need the entire MVC
* `ember-metrics` -- easier way to put google analytics and segment into an app

## Tools to look into

* Lighthouse -- a tool for profiling websites and getting better benchmark feedback
* `ember-bench` -- tool for testing the ember applications
* `pwmetrics` -- not sure, but wanted to look into it
* cardstack.io -- a platform for content management systems

## Ideas

* Use version switchers for documentation. That way users have an easy way to know if something works.
* Look into `hasBlock` and `yield` with `hash` helper for making nested components
