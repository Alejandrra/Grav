---
title: js
---

 <html lang="en">
<head>
 <link rel="stylesheet" href="http://alejandramontenegro.com:86/ejercicio-js" integrity="sha384-1q8mTJOASx8j1Au+a5WDVnPi2lkFfwwEAa8hDDdjZlpLegxhjVME1fgjWPGmkzs7" crossorigin="anonymous">
</head>
<body>
    
Ingrese un numero: <input type="text" id="valor" onkeyup="myFunction()" >
<p id="nombre" style="color:Tomato;"></p>

<script type="text/javascript">
    function myFunction() {

    var max= document.getElementById("valor").value;
    //Imprimir figuras de triangulos formados por asteriscos con ciclo for
    var f,c;
    //triangulo rectangulo recto a derechas

    for (f=1;f<=max;f++)
    {
        for(c=1;c<=f;c++)
            document.write("*");
        document.write("<br>");
    }
    //document.write("<br>");

    //triangulo rectangulo invertido a izquierdas
    for (f=max;f>=1;f--)
    {
        for(c=1;c<=max-f;c++)
            document.write("&nbsp&nbsp");
        for(c=1;c<=f;c++)
            document.write("*");
        document.write("<br>");
    }
    document.write("<br>");
  }
</script>
</body>
</html>