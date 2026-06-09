# Lección 5: Estilo intermedio con CSS (8 minutos)

## Introducción
Para esta quinta lección vamos a ver un poco más sobre CSS, un poco más avanzado.
Tenemos una estructura predefinida: un div con clase "caja" que contiene
un h1 y un párrafo. Para editar esta caja en CSS usamos el punto seguido
del nombre de la clase.

## Propiedades básicas de la caja
Empezamos con algunas propiedades básicas:
- background-color: black → pone el fondo negro
- color: grey → cambia el color de las letras
- max-width: 500px → limita el ancho de la caja
- height: 300px → define la altura de la caja

## Margin
Entre el borde de la caja y la página existe un espaciado en blanco por defecto.
Ese es el margin. Para eliminarlo usamos el selector asterisco que aplica
de manera global:

    * { margin: 0; }

El margin es el espacio entre la caja y lo exterior. Tiene cuatro lados:
margin-top, margin-bottom, margin-left y margin-right.

En vez de escribir los cuatro por separado podemos usar el shorthand:
- margin: 50px → aplica 50px a los cuatro lados
- margin: 50px 100px → el primer valor es arriba/abajo, el segundo es izquierda/derecha
- margin: 50px auto → centra la caja horizontalmente en la página

## Padding
El padding funciona similar al margin pero hacia adentro de la caja.
Mientras el margin agrega espacio afuera, el padding reduce el espacio
disponible para el contenido dentro de la caja.
También tiene sus cuatro lados: padding-top, padding-bottom, padding-left, padding-right.
Para este ejemplo usamos un padding de 30px.

## Border
El border agrega un borde a la caja. Se define con tres valores:
- Grosor: 5px
- Tipo: solid
- Color: grey

Ejemplo: border: 5px solid grey

Además podemos redondear las esquinas con border-radius: 20px.

## Alineamiento del texto
Con text-align controlamos la alineación del texto dentro de la caja:
- text-align: left → alinea a la izquierda
- text-align: center → centra el texto
- text-align: right → alinea a la derecha

## Editar elementos dentro de la caja
Para editar el h1 y el párrafo dentro de la caja, lo correcto es
acceder a ellos a través del nombre de la clase para no afectar
otros elementos del proyecto:

    .caja h1 { ... }
    .caja p { ... }

Para el h1 aplicamos:
- color: white
- margin-bottom: 15px → crea espacio entre el título y el párrafo
- font-size: 32px → tamaño de la letra
- text-align: center → centra el título

Para el párrafo aplicamos:
- font-size: 18px → tamaño de la letra
- line-height: 1.6 → espaciado entre líneas para mejor legibilidad