# Script — Lección 2: Estructura HTML básica (10 minutos)

---

## [INTRO — 0:00 a 0:30]

*Pantalla: título "Estructura HTML básica"*

**Narración:**
En la lección anterior vimos que HTML es el lenguaje que da contenido a los sitios web.
Ahora vamos a aprender cómo se estructura un archivo HTML completo.
Piénsalo como el esqueleto de tu página.

---

## [SECCIÓN 1 — 0:30 a 2:30]
### Las partes de un archivo HTML

*Pantalla: escribir en CodePen, paso a paso*

**Narración:**
Todo archivo HTML empieza con esta línea:

```html
<!DOCTYPE html>
```

*Pantalla: escribir y resaltar `<!DOCTYPE html>`*

**Narración:**
Esto le dice al navegador: "lo que viene a continuación es HTML moderno".
No tienes que memorizar qué significa, solo recuerda que siempre va al inicio.

---

*Pantalla: agregar `<html>`*

**Narración:**
Después viene la etiqueta `<html>`.
Todo el contenido de tu página va dentro de ella.
Las etiquetas tienen una apertura — `<html>` — y un cierre — `</html>`.
El cierre siempre lleva una barra inclinada al inicio.

---

*Pantalla: agregar `<head>` y `<body>`*

**Narración:**
Dentro de `<html>` hay dos secciones principales.

La primera es `<head>`. Aquí va información que el navegador necesita pero que el usuario no ve directamente.
Por ejemplo, el título de la pestaña.

La segunda es `<body>`. Aquí va todo lo que sí se muestra en pantalla: textos, imágenes, botones.

---

## [SECCIÓN 2 — 2:30 a 5:30]
### El título con `<title>`

*Pantalla: escribir dentro de `<head>`*

```html
<head>
  <title>Mi primera página</title>
</head>
```

**Narración:**
Dentro de `<head>` escribimos `<title>`.
Lo que escribas ahí aparece en la pestaña del navegador.
Prueba cambiarlo y mira qué pasa.

---

## [SECCIÓN 3 — 5:30 a 8:00]
### Títulos y párrafos en el `<body>`

*Pantalla: escribir dentro de `<body>`*

```html
<body>
  <h1>Bienvenido a mi página</h1>
  <h2>Sobre mí</h2>
  <p>Me llamo Carlos y me gusta la tecnología.</p>
</body>
```

**Narración:**
`<h1>` es el título más grande e importante. Solo debe haber uno por página.
`<h2>` es un subtítulo, un nivel más pequeño.
Existen hasta `<h6>`, pero los más usados son `<h1>`, `<h2>` y `<h3>`.

`<p>` es un párrafo. Úsalo para cualquier bloque de texto.

*Pantalla: mostrar el resultado en la vista previa de CodePen*

**Narración:**
¿Ves el resultado? Cada etiqueta le dice al navegador cómo mostrar el contenido.

---

## [SECCIÓN 4 — 8:00 a 9:30]
### ¿Qué es un atributo?

*Pantalla: mostrar ejemplo con atributo lang*

```html
<html lang="es">
```

**Narración:**
Los atributos son información extra que le damos a una etiqueta.
Se escriben dentro de la etiqueta de apertura, con el formato `nombre="valor"`.
En este caso, `lang="es"` le dice al navegador que la página está en español.
Veremos más atributos en las próximas lecciones.

---

## [CIERRE — 9:30 a 10:00]

*Pantalla: resumen en texto*
> `<!DOCTYPE html>` siempre va al inicio
> `<html>` contiene toda la página
> `<head>` tiene información del navegador, `<body>` tiene el contenido visible
> `<h1>` al `<h6>` son títulos, `<p>` es un párrafo
> Los atributos dan información extra a las etiquetas

**Narración:**
Ya tienes la estructura base de cualquier página web.
En la siguiente lección agregaremos más elementos: listas, imágenes y enlaces.
Hasta pronto.
