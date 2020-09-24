---
title: lambda calculus interpreter
note: This interpreter (probably...) contains bugs. If you find any, feel free to tell me...
---
- This is a simple lambda-calculus interpreter.
  - Heavily inspired by [lambda-friends](https://nikosai.ml/lambda-friends/)
  - [here](https://github.com/sano-jin/lambda.git) is the code (written in Elm). 
- How to use
  - input an expression and press "run" to run. 
  - to denote a lambda, you can use any one of "\", ™¥™ or ™λ™.
  - e.g.
    - "(\sz.s(sz))(\sz.s(sz))" is as same as "(¥sz.s(sz))(λsz.s(sz))".
  - Space is simpy ignored.
  - One charactor for each variable.
- This not finished yet.
  - It probably contains bugs!
  - I am trying to implement a graph drawing algorithm (instead of just showing a list like now).
    - Please wait.
- twitter[@sano65747676](https://twitter.com/sano65747676)

<script src="lambda.js"></script>
<div id="myapp"></div>
<p> {{ page.note }} </p>
<script>
  var app = Elm.Main.init({
    node: document.getElementById('myapp')
  });
</script>
