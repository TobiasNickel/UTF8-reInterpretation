UTF8-reInterpretation
=====================

make sure that UTF8 specialchars are interpreted right

Sometimes you have the problem that Specialchars are interpreted as something like **Ã„**.
This module makes sure, that these kind of failure get corrected. and **Ã„** is interpreted as an **Ä**.

```JS

var utf8reInterpreter=require("./utf8-reInterpreter.js")

myString="Ã„rzte"; // germany for doctors

console.log(utf8reInterpreter(myString)); // output: Ärzte

```
