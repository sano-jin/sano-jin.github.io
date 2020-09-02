---
title: MOESI Emulator
note: This emulator may (probably...) contain bugs.
---
<html>
<head>
  <meta charset="UTF-8">
  <title>Main</title>
  <script src="main.js"></script>
  <link rel="stylesheet" href="style.css">
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
