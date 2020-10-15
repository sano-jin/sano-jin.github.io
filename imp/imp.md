---
title: IMP interpreter
---
<script src="imp.js"></script>

- This is a simple IMP interpreter.
   - input commands and the initial state, then press "run" to run. 

<div id="myapp"></div>

- Syntax 
  - `a` ::= (arithmetic expression)
    - `n` (integer number)
    - `X` (variable)
    - `a + a` (add)
    - `a * a` (times)
  - `b` ::= (boolean expression)
    - `true` 
    - `false`
    - `a <= a` (less than or equals to)
    - `not b` (not)
    - `b & b` (logical and)
  - `c` ::= (command(s))
    - `skip`   (skip)
    - `X := a` (update)
    - `if b then c else c` (if)
    - `while b do c` (while)
    - `c; c`  (sequence)
  - `s` ::= (state)
    - `{X -> n, ..., X -> n}` (map from variable to int)
  - `Program` ::= (program as a whole)
    - `<c, s>`

- Acknowledgement
  - This interpreter may contains bugs.
- [Source code](https://github.com/sano-jin/imp-interpreter.git) (written in Elm). 
- twitter[@sano65747676](https://twitter.com/sano65747676)
  - Please feel free to contact me.

<script>
  var app = Elm.Main.init({
    node: document.getElementById('myapp')
  });
</script>
