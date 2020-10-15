---
title: MOESI Emulator
---
<script src="main.js"></script>
<link rel="stylesheet" href="style.css">

MOESI is a cache coherence protocol. 
Select Processing Elements (PE), set write/read option and observe their states to change.

<div id="myapp"></div>

- states
  - M : Modified
  - O : Owened
  - E : Exclusive
  - I : Invalid
  - S : Shared
  
- Source code is [here](https://github.com/sano-jin/moesi-emulator)
- Please let me know if you find any bugs.
- Feel free to concact me at
  - twitter[@sano65747676](https://twitter.com/sano65747676)

<script>
  var app = Elm.Main.init({
    node: document.getElementById('myapp')
  });
</script>
