# Functions
Functions, or Methods, or Definations are a basic concept of passing an input to something, and it will return an output. Zircon handles functions similary to that of most languages.

The General Syntax is:
```sh
function meow
	io.write "Meow."
end
```

Here, in this example, the function is named `meow`, and returns nothing or `void` as `io.write` returns `void`, but calls another function. In Zircon, like Ruby or Crystal, parenthesis are not needed for calling functions.  The final call, or value in the scope of the function is returned as the value, or reference. This includes function calls, a function which calls a function at end will return the type or reference of the final function call. For example:
```sh
function meow
	"Meow."
end
```

This returns a string literal with the value "Meow.", the type returned is `String`.