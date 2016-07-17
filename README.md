# advanced-js-notes
1. Named v.s Anonymous function expressionE.g var foo = function bar() { … )

  a) It can self reference itself
  
  b) Easier for debugging (stack trace)

2. ‘this’ rules(take precedence):

  a) `new` binding: turn the function into constructor
  
  `this` binds to itself

  b) hard binding: `function.call(obj)`
  
  `this` binds to `obj`
  
  c) implicit binding rule: context object
  
    `obj.foo()` then `this` bound to `obj`
  
  d) Default binding rule: directly function call
  
    if `strict mode` then `this = undefined`
  
    if `!strict mode` then `this = global`
  
  DETERMINATION:
  ````
  1. was the function called with 'new'
  2. was the function called with 'call' or 'apply'
  3. was the function called via a containing/owning object (context)
  4. DEFAULT: global object (except strict mode)
  ````
