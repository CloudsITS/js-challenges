# JavaScript challenges

The challenges in this repository examine some special features in JavaScript which are
less common in other languages.

Run them e.g. in WebStorm directly, or with node.js from the command line, to see the output.

References:
* **[GP]** *JavaScript: The Good Parts* by Donald Crockford
* **[JP]** *JavaScript Patterns* by Stoyan Stefanov

(*GP:37, Closure* means The Good Parts, Page 37, Chapter about Closure)

#### Closure (access to parent scope)

See *GP:37, Closure* and *JP:107, Private Static Members*

When a variable does not exist in the local scope, the compiler follows the scope tree
up to the top until it finds it there (or not).

    var a = 42;
    function test() {
        console.log( a ); // Prints 42
    }

This allows to implement private variables as well.

#### Invocation

See *JP:64, Callbacks and Scope* and *GP:27, Invocation*

The `this` object is bound to the global object for function calls (different for 
[array functions](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Functions/Arrow_functions)!).

#### Array Functions

See [Array.prototype.map()](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/map),
[Array.prototype.forEach()](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/forEach)
and others.