# Script - Lección 6: Proyecto - Página de perfil (12 minutos)

## Definición del ejemplo

En esta lección el ejemplo será una **tarjeta de perfil personal**. La página integra lo visto en las lecciones anteriores:

- Estructura básica de HTML.
- Títulos, párrafos, listas, imágenes y enlaces.
- Clases para seleccionar elementos.
- Propiedades de CSS como `background-color`, `color`, `font-family`, `max-width`, `margin`, `padding`, `border`, `border-radius`, `text-align` y `line-height`.

Archivos de inicio: `starter-files/lesson-6-profile-starter.html` y `starter-files/lesson-6-profile-starter.css`.
Archivos completos: `completed-examples/lesson-6-profile-complete.html` y `completed-examples/lesson-6-profile-complete.css`.

---

## [INTRO - 0:00 a 0:45]

*Pantalla: título "Proyecto final: Página de perfil personal"*

**Narración:**
Hola. En esta lección vamos a unir todo lo que ya aprendimos para crear una página sencilla pero completa: una tarjeta de perfil personal.
La idea es que puedas cambiar el nombre, la descripción, la foto, las habilidades y el enlace final para hacerla tuya.

Hasta ahora vimos HTML para crear contenido y CSS para darle estilo. Hoy vamos a usar ambas cosas en un solo proyecto.

---

## [SECCIÓN 1 - 0:45 a 2:15]

### Revisar la estructura inicial

*Pantalla: abrir `lesson-6-profile-starter.html`*

**Narración:**
Empezamos con una estructura HTML lista para completar.
Tenemos un `div` con la clase `perfil`. Dentro colocamos una imagen, un título, un subtítulo, un párrafo, una lista de habilidades y un enlace.
En el `<head>` también conectamos el archivo CSS externo:

```html
<link rel="stylesheet" href="lesson-6-profile-starter.css">
```

Esta línea permite mantener el contenido en el HTML y los estilos en un archivo separado.

```html
<div class="perfil">
    <img class="foto-perfil" src="..." alt="Foto de perfil">
    <h1>Tu nombre</h1>
    <p class="rol">Estudiante de desarrollo web</p>
    <p class="descripcion">...</p>
    <ul class="habilidades">
        <li>HTML</li>
        <li>CSS</li>
        <li>Creatividad</li>
    </ul>
    <a class="boton" href="https://developer.mozilla.org/es/" target="_blank">
        Seguir aprendiendo
    </a>
</div>
```

**Narración:**
Fíjate que usamos clases como `perfil`, `foto-perfil`, `rol`, `descripcion`, `habilidades` y `boton`.
Estas clases nos van a permitir aplicar estilos específicos sin afectar toda la página.

---

## [SECCIÓN 2 - 2:15 a 3:45]

### Preparar estilos generales

*Pantalla: abrir `lesson-6-profile-starter.css`*

**Narración:**
Primero quitamos el margen y el padding que el navegador agrega por defecto.
Esto nos ayuda a controlar mejor los espacios.

```css
* {
    margin: 0;
    padding: 0;
}
```

Ahora damos estilo al `body`, que representa toda la página:

```css
body {
    background-color: #e8f3f1;
    color: #1f2937;
    font-family: Arial, sans-serif;
}
```

**Narración:**
Aquí usamos tres propiedades que ya vimos:
`background-color` para el fondo, `color` para el texto y `font-family` para la fuente.

---

## [SECCIÓN 3 - 3:45 a 6:00]

### Crear la tarjeta principal

*Pantalla: completar `.perfil`*

**Narración:**
Ahora vamos a convertir nuestro `div` en una tarjeta.
Para eso usamos la clase `.perfil`.

```css
.perfil {
    max-width: 520px;
    margin: 50px auto;
    background-color: white;
    padding: 30px;
    border: 3px solid #0f766e;
    border-radius: 20px;
    text-align: center;
}
```

**Narración:**
`max-width` limita el ancho de la tarjeta.
`margin: 50px auto` la separa de arriba y la centra horizontalmente.
`padding` crea espacio interno.
`border` agrega un borde.
`border-radius` redondea las esquinas.
Y `text-align: center` centra el contenido.

Con esto ya tenemos la base visual del proyecto.

---

## [SECCIÓN 4 - 6:00 a 7:40]

### Dar estilo a la imagen y textos

*Pantalla: completar `.foto-perfil`, `.perfil h1`, `.rol` y `.descripcion`*

**Narración:**
Ahora hacemos que la imagen parezca una foto de perfil.

```css
.foto-perfil {
    width: 140px;
    height: 140px;
    border-radius: 50%;
    border: 5px solid #0f766e;
}
```

**Narración:**
El `border-radius: 50%` convierte la imagen en un círculo.
Luego editamos el título, el rol y la descripción:

```css
.perfil h1 {
    color: #0f766e;
    margin-top: 20px;
    margin-bottom: 8px;
    font-size: 32px;
}

.rol {
    color: #475569;
    font-size: 18px;
    margin-bottom: 18px;
}

.descripcion {
    font-size: 16px;
    line-height: 1.6;
    margin-bottom: 22px;
}
```

**Narración:**
El `line-height` hace que la descripción se lea mejor porque aumenta el espacio entre líneas.

---

## [SECCIÓN 5 - 7:40 a 10:20]

### Estilizar habilidades y enlace

*Pantalla: completar `.habilidades`, `.habilidades li` y `.boton`*

**Narración:**
La lista de habilidades usa `ul` y `li`, que ya vimos en HTML.
Ahora la vamos a mejorar con CSS.

```css
.habilidades {
    list-style: none;
    margin: 16px 0 24px;
}

.habilidades li {
    background-color: #ccfbf1;
    color: #0f766e;
    margin: 8px auto;
    padding: 10px;
    border-radius: 12px;
    max-width: 240px;
    font-weight: bold;
}
```

**Narración:**
`list-style: none` quita los puntos de la lista.
Cada `li` se convierte en una pequeña etiqueta visual.

Finalmente, convertimos el enlace en un botón:

```css
.boton {
    display: inline-block;
    background-color: #0f766e;
    color: white;
    padding: 12px 20px;
    border-radius: 12px;
    text-decoration: none;
    font-weight: bold;
}
```

**Narración:**
Aunque sigue siendo un enlace, se ve como un botón gracias al fondo, el padding y los bordes redondeados.
`text-decoration: none` quita la línea debajo del enlace.

---

## [SECCIÓN 6 - 10:20 a 11:20]

### Personalizar el proyecto

*Pantalla: cambiar nombre, descripción y habilidades*

**Narración:**
Ahora puedes personalizar la página.
Cambia el nombre por el tuyo, escribe una descripción breve y modifica la lista de habilidades.
Por ejemplo:

```html
<h1>Andrea López</h1>
<p class="rol">Estudiante y futura desarrolladora web</p>
```

**Narración:**
También puedes cambiar los colores del CSS para que la página tenga otro estilo.
Lo importante es mantener la estructura ordenada.

---

## [CIERRE - 11:20 a 12:00]

*Pantalla: mostrar el resultado final*

**Narración:**
Listo. Hoy construimos una página de perfil usando HTML y CSS.
Usamos títulos, párrafos, listas, imágenes, enlaces, clases y propiedades de estilo.

Este proyecto demuestra la idea principal del desarrollo web básico:
HTML crea el contenido y CSS mejora su presentación.

En la siguiente lección vamos a revisar errores comunes y buenas prácticas para que tu página sea más clara y fácil de corregir.
