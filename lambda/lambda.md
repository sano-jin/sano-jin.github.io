---
title: lambda calculus interpreter
note: This interpreter may (probably...) contain bugs.
---
- This is a simple lambda-calculus interpreter.
  - input an expression and press "run" to run. 
  - [here](https://github.com/sano-jin/lambda.git) is the code (written in Elm). 

<script src="lambda.js"></script>
<div id="myapp"></div>
<p> {{ page.note }} </p>
<script>
  var app = Elm.Main.init({
    node: document.getElementById('myapp')
  });
</script>
