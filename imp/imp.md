---
title: pi calculus interpreter
---
<script src="imp.js"></script>

- This is a simple IMP interpreter.
   - input commands and the initial state then press "run" to run. 

<div id="myapp"></div>

- Syntax 
  - `P`, `Q` =
    - `x!y` (Send the value y over channel x)
    - `x?y.P` (Receive on channel x, bind the result to y, then run P)
    - `P|Q` (run P and Q simultaneously)
    - `\x.P` (create a new channel x and run P)
    - `!P` (NOT implemented yet. Repeatedly spawn copys of P)
    - `0` (Terminate the process)
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
