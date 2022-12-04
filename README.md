# clicker
An example of a clicker game with multiplier and CPS.

Made by [AwesomePotatoCodes](https://github.com/AwesomePotatoCodes)! All I did was polish it a bit and get some stuff working.

Here's what I changed:
* Added `type="image/png"` to favicon `<link>` (totally optional, but why not)
* Fixed the issue I _think_ you were having with the enter key hack prevention overriding the other keys you wanted to prevent
* Amogus
* Wrapped individual counter values (like click count and CPS) with their own `<span>` to make it a lot neater to update their values; I forced `<span>` to inherit the parent styles to keep the bold from the `<p>` element, so that should still be the same
* Moved some global variables to functions and fixed some incorrectly defined variables that would have caused issues at some point
* Changed some function names and arguments for better readability and consistency
* Simplified the `addCPS()` function so it only does what it needs to do
* Moved the screen refresh to its own `refresh()` function, makes it so much easier to do!
* Changed things like `clicks = clicks + cpc` to `clicks += cpc`, this achieves the same addition with less repetitive code (`+=` basically adds whatever you specify to the variable instead of overwriting it, `-=` does the same but for subtraction)
* Changed a few stray `=` to `===` where they should be, changed `==` to `===` for more precise matching (`===` matches the value _and_ type, good practice for something like this that uses both numbers and strings)
* Formatted for ease of access

I think that's it, let me know if you notice anything unusual!
