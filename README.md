# 2nd edition - Get Started - Chapter 1

## What's With That Name
- real name: ECMAScript

<br>

## Language Specification
- TC39 manages the language specification, that is consequently submitted to ECMA
- TC39 has 5 stages, 0 is initial stage and 4 is something eligible to be included in the lang

<br>

## The Web Rules Everything About (JS)
- The browsers can't introduce every features the ECMA wants. If a new feature breaks some websites, ECMA possibly changes that.
- Sometimes ECMA doesn't change a browser-braking features, and so the JS specification and the implementation may differ a bit.
- The runtimes, since don't have the problems a browser can have, are forced to implement the whole specification.

<br>

## Not All (Web) JS...
- a JS environment (a browser for example) can add some APIs in the global scope (like fetch, alert)

<br>

## It's Not Always JS
- a JS REPL it doesn't handle the code like a JS engine handles a .js file

<br>

## Many Faces
- JS is multi-paradigm

<br>

## Backwards & Forwards
- JS is 99.9% backward compatible (old code works in new versions of engines) because old websites can't break.

<br>

## Jumping the Gaps
- JS is not forward compatible (new code doesn't work in old engines) and so we can use tools like Babel: it transpiles the new JS version code to an old JS version code in order to make this new code be then compatible with the old engine.

<br>

## Filling the Gaps
- What happens if I want to provide forward compatibility for an engine native API? I can create a polyfill: when transpiling the code for an old engine version I provide an implementation for this missing new API using a valid old syntax to simulate the new API. 
- For example: the promise method ```finally``` doesn't exist in a pre ES2019 engine, and so if I want to use this method in a ES2015 engine, during the transpilation I need to provide a fallback implementation with valid ES2015 syntax.

example

```
// ES2019 new method
if (!Promise.prototype.finally) {
  // provide an implementation with valid ES2015 syntax
}
```

<br>

## What's in an Interpretation?

<br>

## Web Assembly (WASM)

<br>

## Strictly Speaking
