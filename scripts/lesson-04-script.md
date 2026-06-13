# Script — Lección 4: Introducción a CSS (10 minutos)

---

## [INTRO — 0:00 a 0:30]

*Pantalla: título "Introducción a CSS"*

**Narración:**
En las lecciones anteriores aprendiste a darle estructura a una página con HTML.
Pero seguramente notaste algo: todo se ve aburrido, en blanco y negro, sin estilo.
Eso es exactamente lo que CSS viene a solucionar.
CSS es el lenguaje que le da color, fuente y diseño a tu página.

---

## [SECCIÓN 1 — 0:30 a 2:30]

### Vincular CSS a tu HTML

*Pantalla: mostrar el archivo `index.html` en CodePen, enfocado en el `<head>`*

**Narración:**
CSS puede escribirse de distintas formas, pero la más ordenada y profesional
es tener un archivo separado — normalmente llamado `styles.css` — y conectarlo a tu HTML.
Para eso usamos esta línea dentro del `<head>`:

```html
<link rel="stylesheet" href="styles.css">
```

*Pantalla: escribir la línea `<link>` dentro del `<head>` y resaltarla*

**Narración:**
`link` le dice al navegador: "conecta este archivo externo a mi página".
`rel="stylesheet"` indica que es una hoja de estilos.
`href="styles.css"` es la ruta al archivo CSS, igual que cuando vimos los enlaces.

A partir de ahora, todo lo que escribas en `styles.css` va a afectar tu página.
Vamos a comprobarlo.

---

## [SECCIÓN 2 — 2:30 a 5:00]

### Selectores: ¿a qué elemento le aplicamos el estilo?

*Pantalla: cambiar al panel CSS en CodePen*

**Narración:**
Antes de cambiar colores o fuentes, necesitamos decirle a CSS
a qué parte de la página queremos aplicar el estilo.
Eso se hace con los **selectores**.

El selector más básico es el de etiqueta. Por ejemplo:

```css
h1 {

}
```

*Pantalla: escribir el selector `h1 {}` en el CSS*

**Narración:**
Esto significa: "aplica estos estilos a todos los `<h1>` de la página".
Dentro de las llaves escribimos las propiedades.

---

*Pantalla: agregar un selector de clase*

**Narración:**
También podemos crear nuestras propias categorías usando **clases**.
En el HTML, agregamos un atributo `class` a la etiqueta que queremos:

```html
<p class="destacado">Este texto es especial.</p>
```

Y en el CSS, nos referimos a esa clase con un punto antes del nombre:

```css
.destacado {

}
```

*Pantalla: escribir `.destacado {}` en el CSS y resaltar el punto*

**Narración:**
El punto es clave — sin él, CSS no entendería que estás hablando de una clase.
Las clases son útiles cuando quieres aplicar el mismo estilo a varios elementos distintos.

---

## [SECCIÓN 3 — 5:00 a 7:30]

### `color` y `background-color`

*Pantalla: cursor dentro del selector `h1 {}`*

**Narración:**
Ahora sí, vamos a darle color a la página.
La propiedad `color` cambia el color del texto:

```css
h1 {
  color: steelblue;
}
```

*Pantalla: escribir `color: steelblue;` y mostrar el resultado en la vista previa*

**Narración:**
¿Ves cómo el título cambió de color al instante?
Puedes usar nombres en inglés como `red`, `green`, `orange`, `purple`...
o códigos de color hexadecimales para colores más exactos, como `#e74c3c`.

---

*Pantalla: agregar `background-color` al `body`*

**Narración:**
Ahora la propiedad `background-color` cambia el color de fondo de un elemento.
Vamos a cambiar el fondo de toda la página:

```css
body {
  background-color: #f0f4f8;
}
```

*Pantalla: escribir la propiedad y mostrar el resultado*

**Narración:**
También puedes aplicar `background-color` a cualquier elemento,
no solo al `body`. Prueba aplicarlo a un `<section>` o a un `<p>`.

*Pantalla: aplicar `background-color` a `.destacado` y mostrar resultado*

---

## [SECCIÓN 4 — 7:30 a 9:30]

### `font-family`: cambiar la fuente

*Pantalla: cursor dentro del selector `body {}`*

**Narración:**
La última propiedad de hoy es `font-family`, que cambia el tipo de letra.
Si la aplicamos al `body`, afecta a toda la página:

```css
body {
  background-color: #f0f4f8;
  font-family: Arial, sans-serif;
}
```

*Pantalla: escribir `font-family: Arial, sans-serif;` y mostrar el resultado*

**Narración:**
¿Por qué ponemos dos fuentes separadas por coma?
La primera — `Arial` — es la que queremos usar.
La segunda — `sans-serif` — es el plan B: si el navegador no tiene Arial,
usará cualquier fuente sans-serif que tenga disponible.
Siempre es buena práctica poner ese plan B.

---

*Pantalla: cambiar a una fuente diferente, por ejemplo `Georgia, serif`*

**Narración:**
Prueba cambiando a `Georgia, serif` y mira la diferencia.
Las fuentes `serif` tienen pequeños adornos en las letras.
Las `sans-serif` son más limpias y modernas.

---

## [CIERRE — 9:30 a 10:00]

*Pantalla: resumen en texto*

> `<link rel="stylesheet" href="styles.css">` conecta tu CSS con tu HTML
> Los selectores definen a qué elemento aplicas el estilo
> `.clase` selecciona elementos con ese atributo `class`
> `color` cambia el color del texto
> `background-color` cambia el color de fondo
> `font-family` cambia el tipo de letra

**Narración:**
Ahora tu página ya tiene personalidad.
En la siguiente lección vamos a seguir dando estilo:
márgenes, bordes y cómo centrar contenido.
Hasta pronto.
