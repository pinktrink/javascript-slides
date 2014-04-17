# JavaScript
## Things you should know
* Functional programming
    * Javascript is **not** purely functional
    * Some characteristics of functional languages
        * First-class functions
        * High-order functions
    * Understand function scoping
    * Define functions outside of loops
        * V8 issues with in-place definition
        * Functional languages declare functions in outer scope
    * Determinism
    * Some languages that are functional or can be functional
        * Haskell
        * OCaml
        * Erlang (not by design)
        * Python
* ECMA-262 Edition 5
    * Should I drop ECMAScript 3?
        * IE 8 is almost out of the picture, taking ECMAScript 3 with it
    * Syntax changes
        * Object literal getters and setters
    * Don't be afraid of the prototype
        * for-in prototypical iteration
        * `Object.defineProperty` / `Object.defineProperties`
            * IE 8 issue
    * Functional programming with ECMAScript 5
        * Function currying with `Function.prototype.bind`
        * Array iteration
            * `Array.prototype.forEach`
            * `Array.prototype.map`
            * `Array.prototype.filter`
            * `Array.prototype.reduce`
            * Caveats
            * Avoiding over-iteration
    * Start using strict mode
        * Scoping for strict evaluation
        * No assigning variables without var
        * No assigning immutable properties
        * No deleting non-deletable properties
        * No defining the same property twice in objects
        * No defining the same argument twice in functions
        * No prefixing numbers with 0
        * No `with`
        * `undefined` is immutable
    * Stop using `arguments.callee`
    * Libraries have their place
        * Uses for animation
            * Can it be replaced with CSS3?
        * Cross-browser compatibility
            * Is that even a problem anymore?
            * Can you just use `Array.prototype.forEach`?
        * How much of the library are you using?
        * jQuery 2
        * Lodash
            * `_.isUndefined`
                * String comparison of `typeof`
                    * Same performance as `===`
                * In strict mode, `undefined` is immutable and safe for comparison
* JavaScript Oddities
    * `delete`
        * Returns `true` or `false`
        * Effects on `Array.length`
        * No deleting variables
            * Variables defined by `eval` can be deleted
    * `eval`
        * Direct `eval` evaluates within the current scope
        * Indirect `eval` evaluates in the global scope
        * **DO NOT USE EVAL**
    * Objects
        * Scalar vs multi-dimensional
        * `===`
        * Everything is an object
            * Array indices are cast to strings
    * Q/A
