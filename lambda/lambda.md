---
title: lambda calculus interpreter
note: This interpreter (probably...) contains bugs. If you find any, feel free to tell me...
---
<script src="lambda.js"></script>

- This is a simple lambda-calculus interpreter.
   - input an expression and press "run" to run. 
   - [here](https://github.com/sano-jin/lambda.git) is the code (written in Elm). 

<div id="myapp"></div>

- How to use
  - to denote a lambda, you can use any one of `\`, `¥` or `λ`.
  - e.g.
    - `(\sz.s(sz))(\sz.s(sz))` is as same as `(¥sz.s(sz))(λsz.s(sz))`.
  - Space is simpy ignored.
  - One charactor for each variable.
- Acknowledgement
  - This is heavily inspired by [lambda-friends](https://nikosai.ml/lambda-friends/)
  - This not finished yet.
    - It probably contains bugs!
      - Please tell me if you find any.
    - I am trying to implement a graph drawing algorithm (instead of just showing a list like now).
      - Please wait.
- twitter[@sano65747676](https://twitter.com/sano65747676)


<script>
  var app = Elm.Main.init({
    node: document.getElementById('myapp')
  });
</script>
