# Higher Order Components

Speaker: Miguel Camba

Basically the same idea as higher order functions -> functions that call functions.

Can use the hash helper to make components that are nested.

e.g.

```js
(hash somevalue=(component stuff) othervalue=(compnent stuff))
```

Look at the `hasBlock` magic value to know if you sould do it.


## Takeaway

* Look into using these `hasBlock` and the "inner components"
* Hash helper with `yield` makes the nested components much better/easier
