---
title: pi calculus interpreter
---
<script src="imp.js"></script>

- This is a simple IMP interpreter.
   - input commands and the initial state then press "run" to run. 

<div id="myapp"></div>

- Syntax 
  - `a` ::=
    - `n` (integer number)
    - `X` (variable)
    - `a + a` (add)
    - `a * a` (times)
  - `b` ::=
    - `true` 
    - `false`
    - `a <= a` (less than or equals to)
    - `not b` (not)
    - `b & b` (logical and)
  - `c` ::=
    - `skip`   (skip)
    - `X := a` (update)
    - `if b then c else c` (if)
    - `while b do c` (while)
    - `c; c`  (sequence)
  - `s` ::=
    - `{X -> n, ..., X -> n}` (map from variable to int)
  - `Program` ::=
    - `<c, s>`

- How to use
- Acknowledgement
  - This is heavily inspired by [lambda-friends](https://nikosai.ml/lambda-friends/).
- [Source code](https://github.com/sano-jin/imp-interpreter.git) (written in Elm). 
- twitter[@sano65747676](https://twitter.com/sano65747676)
  - Please feel free to contact me.

<script>
  var app = Elm.Main.init({
    node: document.getElementById('myapp')
  });
</script>
