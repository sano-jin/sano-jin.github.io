---
title: pi calculus interpreter
---
<script src="lambda.js"></script>

- This is still in the middle of implementation.
  - You can NOT use this. Please wait...

- This is a simple pi-calculus interpreter.
   - input an expression and press "run" to run. 

<div id="myapp"></div>

- Syntax
  - P, Q =
    - x!y.P (Send the value y over channel x, then run P)
    - x?y.P (Receive on channel x, bind the result to y, then run P)
    - P|Q (run P and Q simultaneously)
    - \x.P (create a new channel x and run P)
    - !P (Repeatedly spawn copys of P)
    - 0
- How to use
  - to denote a lambda, you can use any one of `\`, `¥` or `λ`.
  - e.g.
    - `(\sz.s(sz))(\sz.s(sz))` is as same as `(¥sz.s(sz))(λsz.s(sz))`.
  - Space is simpy ignored.
  - One charactor for each variable.
- Acknowledgement
  - This is heavily inspired by [lambda-friends](https://nikosai.ml/lambda-friends/).
  - This not finished yet.
    - It probably contains bugs!
      - Please tell me if you find any.
    - I am trying to implement a graph drawing algorithm (instead of just showing a list like now).
      - Please wait.
    - I do know the design of this page sucks! :-)     
- [Source code](https://github.com/sano-jin/lambda.git) (written in Elm). 
- twitter[@sano65747676](https://twitter.com/sano65747676)
  - Please feel free to contact me.

<script>
  var app = Elm.Main.init({
    node: document.getElementById('myapp')
  });
</script>
