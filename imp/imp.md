---
title: IMP Interpreter
---
<link href="https://fonts.googleapis.com/css2?family=Inconsolata&display=swap" rel="stylesheet">
<link rel="stylesheet" href="style.css">

# IMP Interpreter

IMP is a tiny imperative language specially designed for giving a formal description on execution of a program: Operational Semantics. 

Input commands and an initial state then press run to see the derivation tree (based on big-step semantics).

<div id="myapp"></div>
<div id="derivationTree"></div>

## Syntax 
- `a` ::= (arithmetic expression)
  - `n` (integer number)
  - `X` (variable)
  - `a + a` (add)
  - `a * a` (times)
- `b` ::= (boolean expression)
  - `true` 
  - `false`
  - `a <= a` (less than or equals to)
  - `not b` (not)
  - `b & b` (logical and)
- `c` ::= (command(s))
  - `skip`   (skip)
  - `X := a` (update)
  - `if b then c else c` (if)
  - `while b do c` (while)
  - `c; c`  (sequence)
- `s` ::= (state)
  - `{X -> n, ..., X -> n}` (map from variable to int)
- `Program` ::= (program as a whole)
  - `<c, s>`

## Acknowledgement
This interpreter may contains bugs.

## Links

- [Source code](https://github.com/sano-jin/imp-interpreter.git) (written in Elm). 
- twitter[@sano65747676](https://twitter.com/sano65747676)
  - Please feel free to contact me.


<link rel="stylesheet" href="./proofTree/proofTree.css">
<script src="./proofTree/proofTree.js"></script>
<script src="imp.js"></script>
<script>
  var app = Elm.Main.init({
    node: document.getElementById('myapp')
  });
  
  app.ports.sendData.subscribe( ( data ) => {
  console.log("Data from Elm: ", data);
  
  const tree = document.getElementById( "derivationTree" );

  if ( data === "error" ) tree.textContent = ""; 
  else renderProofTree( tree, data );
  
  });
</script>
