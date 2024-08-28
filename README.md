# POSITION

1. La página inicial

    1. 
    
    ```html
    <!DOCTYPE html>
    <html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <link rel="stylesheet" href="assets/css/style.css">
        <link rel="stylesheet" href="assets/css/position.css">
        <title>POSITION CSS</title>
    </head>
    <body>

        <div class="contenedor">
            <div class="caja caja-1">1</div>
            <div class="caja caja-2">2</div>
            <div class="caja caja-3">3</div>
            <div class="caja caja-4">4</div>
            <div class="caja caja-5">5</div>
            <div class="caja caja-6">6</div>        
        </div>
    </body>
    </html>
    ```
    2. El html anterior nos muestra que tenemos un contenedor div y 6 cajas, cada una con 2 clases, una clase general llamada caja y otra clase invidual para cada una, llamadas caja-1, caja-2, caja-3, caja-4, caja-5 y caja-6.

2. El estilo CSS para el archivo style.css

    1. 

    ```CSS
    html, body{
        margin:0;
        padding:0;
        box-sizing: border-box;
    }

    .contenedor{
        margin:20vh auto;  
        border:5px solid black;     
        width: 300px; 
    }

    .caja{
        width:100px;
        height: 100px;
        text-align: center;
        color:white;
    }

    .caja-1{
        background-color: #FF6961;
    }

    .caja-2{
        background-color: #77dd77;
    }
    .caja-3{
        background-color: #E79EFF;
    }
    .caja-4{
        background-color: #84B6F4;
    }
    .caja-5{
        background-color: #EE7F41;
    }
    .caja-6{
        background-color: #5E704A;
    }
    ```

    2. El estilo configura en las etiquetas HTML y BODY margen:0, padding:0 y la configuración de box-sizing: border-box;

    3. La clase .contenedor tiene:
        1.  Para el div esta configurada con un margin: 20vh auto; lo que quiere decir que tiene una margen de 20 viewport de alto y auto (centrado) en el viewport ancho.
        2. El div tiene un borde de 5px solid black.
        3. El div tiene un ancho de 300px.¨
    4. La clase .caja tiene:
        1. width:100px;
        2. height: 100px;
        3. text-align: center;
        4. color:white;
    5. Las cajas caja-1, caja-2, caja-3, caja-4 y caja-5 tienen un background-color individual por cada una.

3. Con lo cual logramos:
<img src= "assets/img/imagen1.jpg" alt="Muestra position" style="border: 2px solid grey;">

4. 2. El estilo CSS para el archivo position.css


Las propiedades que encontramos son:

1. static: 
    1. Es el valor por defecto de todas las cajas que tenemos, por lo tanto no podemos realizar ningun cambio en la posición de los elementos. 
    2. Con la propiedad static no funcionan las propiedades top, left, bottom y right.
    3. Esto quiere decir que con la propiedad static el navegador coloca las cajas o elementos siguiendo el flujo de HTML.

2. relative: 
    1. Es la posición relativa a la caja donde se encuentra o elemento padre.
    2. La caja con proiedad relative  se mueve teniendo en cuenta las propiedades top, left, bottom y right. 
    3. Si se tienen registradas las propíedades top y left, las propiedades right y bottom no funcionan. Prevalecen siempre las propiedaes top y left.
    4. Se pueden utilizar valores negativos.

3. absolute:
4. fixed:
5. sticky:
6. z-index:

ver manual en  https://www.youtube.com/watch?v=_e0ddNlc0Y8&t=1s
