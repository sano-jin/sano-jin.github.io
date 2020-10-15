---
title: MOESI Emulator
---
<script src="main.js"></script>
<link rel="stylesheet" href="style.css">

<div id="myapp"></div>
MOESI is a cache coherence protocol. Select Processing Elements (PE), set write/read option and observe their states to change.

- states
  - M : Modified
  - O : Owened
  - E : Exclusive
  - I : Invalid
  - S : Shared
  
- Source code is [here](https://github.com/sano-jin/moesi-emulator)
- Please let me know if you find any bugs.
- Feel free to concact me
  - twitter@[sano](https://twitter.com/sano65747676)

<script>
  var app = Elm.Main.init({
    node: document.getElementById('myapp')
  });
</script>
