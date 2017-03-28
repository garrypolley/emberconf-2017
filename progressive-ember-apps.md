# Progressive Ember Apps

Progressive web applications load all the time and fast.

Allow web access on mobile access on a device. Applications are not
directly relevant for most applications. (Garry interpretation for now)

## Needs for apps

* Must look good on mobile
* Installs on device
* Works offline
* Works fast

Trello is a good example of having native and web.

### Looks good

* Take a look at trello, it can be done
* Be responsive

### Install on device

* Use an app manifest
* Save to the home screen to get a "real" app -- only chrome supports app manifest
* iOS requires some meta tags for app install stuff
* Windows also supports the same sort of stuff
* `ember-web-app` and config makes this all "just work" -- Yay addons! `config/manifest.js`

### Works offline

* Use a service worker
* Save assets on install via the service worker
* Intercept requests with the service worker
* Background syncing can happen via syncs
* Can do push notifications within these service workers -- that'll be nice
* `ember-service-worker` and `broccoli-serviceworker` both help make the service workers work
* `ember-service-worker` allows for easy plugin, add
  * `ember-service-worker-index`
  * `ember-service-worker-asset-cache`
  * `ember-service-worker-cache-fallback`
* `broccoli-serviceworker` allows for setting up application
  * Need to setup via a configuration file
* These two things help with working offline
* Application cache is the "best bet" for getting the application to work offline -- this is not flexible
  * `broccoli-manifest` allows for easy application cache use, can use the `app/config/environment.js` to setup stuff
* Local storage is a good place for holding data
  * Addons for this stuff `ember-localstorage-adaptor`
* Local storage for `ember-localstorage-adaptor`
* Local storage++ for `ember-localforage-adapter` uses other fancy stuff like indexDb
* `ember-pouch` will sync with other `pouchdb` on a server for you, kind of cool

### Works fast

* Native is showing content faster in this first example -- therefore, look into first page render
* `ember-cli-fastboot` server side rendering, it'll be a little faster, still in beta
* Second page render is helped via the service worker and the app cache
* `ember-engines` helps for lazy loading and smaller apps, you can have "sub-apps" as needed


## Tools

* `Lighthouse` will run some tests to tell you how your app is doing for progressive web app


## Conclusions

* It is possible, to not do native mobile and have good mobile experience
* Ember can support these dreams, and it does make it easier than doing it alone


## Idea I had

* Maybe use some of this to make my blog work offline and online, Maybe even have edits?
* Would still publish to github, but the underlying bits could be managed via local storage, and I could upload json files of my actual data
