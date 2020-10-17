---
title: lambda calculus interpreter
note: This interpreter (probably...) contains bugs. If you find any, feel free to tell me...
---

Lambda calculus is an absolute foundation of Functional programming languages.
It is simple yet powerful enough to encode ALL the programs run on computers (as same as Turing Machine).

Input an expression and press run to get the full reduction graph.

<div id="myapp"></div>

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

<script src="lambda.js"></script>
<script>
  var app = Elm.Main.init({
    node: document.getElementById('myapp')
  });
</script>
