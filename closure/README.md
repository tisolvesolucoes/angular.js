This file contains externs for use with the Closure compiler (aka JSCompiler).
Passing these files to the --externs parameter of a compiler pass allows using
type annotations for AngularJS objects. For example, Angular's $scope objects
can be annotated as:
  /** @type {angular.Scope} */ var scope = $scope;

This allows JSCompiler to type check accesses to scope, give warnings about
missing methods or incorrect arguments, and also prevents renaming of property
accesses with advanced compilation.

The externs are incomplete and maintained on an as-needed basis, but strive to
be correct. Externs for individual modules should be added in separate files.

See https://developers.google.com/closure/compiler/
