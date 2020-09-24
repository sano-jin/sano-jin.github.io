---
title: lambda calculus interpreter
note: This interpreter (probably...) contains bugs. If you find any, feel free to tell me...
---
- This is a simple lambda-calculus interpreter.
  - input an expression and press "run" to run. 
  - [here](https://github.com/sano-jin/lambda.git) is the code (written in Elm). 
- This not finished yet.
  - It probably contains bugs!
  - I am trying to implement graph drawing algorithm (instead of just showing list like now)
    - Please wait
    
<script src="lambda.js"></script>
<div id="myapp"></div>
<p> {{ page.note }} </p>
<script>
  var app = Elm.Main.init({
    node: document.getElementById('myapp')
  });
</script>
