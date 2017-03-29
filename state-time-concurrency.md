# State time concurrency

Speaker: Alex Matchneer

Sate, time, and concurrency

* State is the "place" of the app
* Time is when the state happens
* Concurrency is any set of state and time that occures at the same time

## Async stuff

* Concurrency causes multiple states of an async action
* Button mashing in a UI is a good example

## Real talk

* Bargained with designer to not do feature because issues with framework.  :-(  Ember-Concurrency can help


What is `ember-concurrency`?

It's a task primitive. Gives better syntax for async operations, helps with cancel actions. Also comes with a lot of derived state

## Derived State

* It helps you not have to keep track of a lot of `bool` values for state management
* `isRunning` is one of them, says that the async function is still running
* `.last` and `.lastSuccessful` are nice for getting most recent or most successful `.last` seems nice for loading stuff

Helps with 4th dimension of time when managing state.
