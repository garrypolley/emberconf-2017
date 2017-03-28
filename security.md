# Security

speaker: @ingridepure

## Attacks

* There was a GIFAR attack by putting a `jar` in a `gif`
* `IMA(G)JS` attach, putting executable code inside the `jpeg` (`.php`) causes some of this to happen
  * (Garry thoughts) -- seems like this could be avoided by using content negotiation correctly

First rule of web securty -- NEVER trust user data, EVER!

## What to know aobut

* User Input
* Same Origin Policy
* Content Security Policy
* Browser Security Features
* HTML as input in Ember

Ember by default escapes all HTML, unless you tell it otherwise.

`ember-cli-content-security-policy`(use CSP V2 and V3 only) -- look at this of the bits that are whitelists on browsers

Look at htps://content-security-policy.com/


* Avoid HTMLSafe in ember code
* https://embermap.com/topics/contextual-components <-- this may help with components that have sections, way better than what I'm doing now
* Write good helpers, prefer updating the existing DOM over making new ones
  * For example, a `mailto` helper that creates DOM nodes via the create element API
* Avoid using `_blank` for target on its own. Be sure to use the `noopener`/`noreferer` stuff on there
  * The `rel`  for this: `rel="noopener noreferer"`
  * Checkout `ember-template-lint` for looking at our templates
  * `link-rel-noopener`: `strict` for a lint setting
