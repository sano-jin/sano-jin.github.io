---
title: lambda calculus interpreter
note: This interpreter may (probably...) contain bugs.
---
<script src="lambda.js"></script>
<div id="myapp"></div>
<p> {{ page.note }} </p>
<script>
  var app = Elm.Main.init({
    node: document.getElementById('myapp')
  });
</script>
