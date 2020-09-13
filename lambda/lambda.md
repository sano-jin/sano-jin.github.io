---
title: lambda calculus interpreter
note: This interpreter may (probably...) contain bugs.
---
<html>
<head>
  <meta charset="UTF-8">
  <title>Main</title>
  <script src="lambda.js"></script>
</head>

<body>
  <div id="myapp"></div>
  <p> {{ page.note }} </p>
  <script>
  var app = Elm.Main.init({
    node: document.getElementById('myapp')
  });
  </script>
</body>
</html>