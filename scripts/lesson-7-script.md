# Script - Lección 7: Errores comunes y próximos pasos (5 minutos)

## Definición del ejemplo

En esta lección se revisa una versión con errores de la misma tarjeta de perfil personal creada en la lección 6. El objetivo no es construir una página nueva, sino aprender a detectar y corregir problemas frecuentes.

Archivos con errores: `starter-files/lesson-7-debug-starter.html` y `starter-files/lesson-7-debug-starter.css`.
Archivos corregidos: `completed-examples/lesson-7-debug-complete.html` y `completed-examples/lesson-7-debug-complete.css`.
Para CodePen, usar `starter-files/lesson-7-debug-codepen.html` en el panel HTML y `starter-files/lesson-7-debug-starter.css` en el panel CSS.

Errores que se corrigen en el video:

- Clase escrita diferente en HTML y CSS.
- Propiedad CSS mal escrita.
- Imagen sin atributo `alt`.
- Etiqueta `h1` sin cerrar.
- Enlace sin `https://`.

---

## [INTRO - 0:00 a 0:30]

*Pantalla: título "Errores comunes y próximos pasos"*

**Narración:**
Hola. En esta última lección vamos a hacer algo muy importante: revisar errores.
Cuando una página no se ve como esperamos, normalmente no significa que todo esté mal.
Muchas veces es un detalle pequeño: una etiqueta sin cerrar, una clase mal escrita o un enlace incompleto.

Vamos a corregir una versión con errores de nuestra página de perfil.

---

## [SECCIÓN 1 - 0:30 a 1:20]

### Error 1: la clase no coincide

*Pantalla: mostrar `.perfil-card` en el panel CSS y `<div class="perfil">` en el panel HTML de CodePen*

**Narración:**
El primer error está en las clases.
En HTML tenemos:

```html
<div class="perfil">
```

Pero en CSS aparece:

```css
.perfil-card {
```

**Narración:**
CSS busca una clase llamada `perfil-card`, pero el HTML tiene una clase llamada `perfil`.
Como los nombres no coinciden, el estilo no se aplica.
La solución es escribir el mismo nombre en ambos lugares.

```css
.perfil {
```

---

## [SECCIÓN 2 - 1:20 a 2:05]

### Error 2: propiedad CSS mal escrita

*Pantalla: mostrar `border 3px solid #2563eb;`*

**Narración:**
El segundo error está en esta línea:

```css
border 3px solid #2563eb;
```

Falta el signo de dos puntos después de `border`.
En CSS, casi siempre escribimos:

```css
propiedad: valor;
```

Entonces corregimos la línea así:

```css
border: 3px solid #2563eb;
```

---

## [SECCIÓN 3 - 2:05 a 3:00]

### Error 3: etiqueta sin cerrar

*Pantalla: mostrar el `h1` incompleto*

**Narración:**
El tercer error está en el título.
Tenemos:

```html
<h1>Mi perfil personal
```

Pero falta cerrar la etiqueta.
Debe quedar así:

```html
<h1>Mi perfil personal</h1>
```

**Narración:**
Cuando una etiqueta queda abierta, el navegador puede mezclar elementos y mostrar la página de forma extraña.
Por eso conviene revisar pares de apertura y cierre.

---

## [SECCIÓN 4 - 3:00 a 3:45]

### Error 4: imagen sin texto alternativo

*Pantalla: mostrar el `img` sin `alt`*

**Narración:**
La imagen se muestra, pero le falta el atributo `alt`.
El `alt` describe la imagen si no carga o si una persona usa un lector de pantalla.

```html
<img class="foto-perfil" src="..." alt="Foto de perfil">
```

**Narración:**
No cambia mucho visualmente, pero hace que la página sea más clara y accesible.

---

## [SECCIÓN 5 - 3:45 a 4:30]

### Error 5: enlace incompleto

*Pantalla: mostrar `href="developer.mozilla.org/es/"`*

**Narración:**
El último error está en el enlace.
Si escribimos solo:

```html
href="developer.mozilla.org/es/"
```

el navegador puede interpretarlo como una ruta dentro de nuestro propio sitio.
Para enlazar a otra página web, escribimos la dirección completa:

```html
href="https://developer.mozilla.org/es/"
```

---

## [CIERRE - 4:30 a 5:00]

*Pantalla: mostrar la página corregida*

**Narración:**
Hoy revisamos cinco errores comunes:
clases que no coinciden, propiedades CSS mal escritas, etiquetas sin cerrar, imágenes sin `alt` y enlaces incompletos.

Como próximo paso, puedes personalizar tu página, validar tu HTML y seguir practicando con la documentación de MDN.

Lo importante es no memorizar todo, sino aprender a observar, probar y corregir.
