# Lección 3 — Elementos HTML comunes: títulos, párrafos, listas, imágenes y enlaces

**Duración estimada**: 12 minutos  
**Público**: Estudiantes de 12 a 17 años sin experiencia previa

---

## Contenido teórico

En la lección anterior aprendimos que HTML tiene etiquetas de apertura y cierre, y que todo lo visible va dentro del `<body>`. Ahora vamos a llenar ese body con contenido real: textos, listas, fotos y links. ¡Tu página va a empezar a verse como un sitio web de verdad!

---

### ¿Cómo pongo títulos en mi página?

Imagina que estás escribiendo un libro. Tiene un **título grande** en la portada, luego **capítulos** con títulos más pequeños, y dentro de cada capítulo puede haber **secciones**. En HTML funciona igual: usamos las etiquetas `<h1>` hasta `<h6>` para crear títulos de distintos tamaños.

- `<h1>` es el título más grande e importante (como el título del libro).
- `<h2>` es un subtítulo (como el nombre de un capítulo).
- `<h3>`, `<h4>`, `<h5>`, `<h6>` son títulos cada vez más pequeños.

```html
<h1>Mi Animal Favorito</h1>
<h2>Datos curiosos</h2>
<h3>Alimentación</h3>
```

> **Regla importante**: Solo debe haber **un `<h1>` por página**. Es como el título principal de tu libro: solo hay uno. Los demás (`<h2>`, `<h3>`, etc.) puedes repetirlos cuantas veces necesites.

---

### ¿Cómo escribo texto normal?

Para escribir párrafos de texto usamos la etiqueta `<p>` (de *paragraph* en inglés). Cada bloque de texto que quieras separar va dentro de su propia etiqueta `<p>`.

```html
<p>Los delfines son mamíferos marinos muy inteligentes.</p>
<p>Se comunican entre sí usando silbidos y clics.</p>
```

Piensa en cada `<p>` como un párrafo en un ensayo escolar: cuando cambias de idea o tema, abres un nuevo párrafo.

---

### ¿Cómo hago listas?

¿Alguna vez has hecho una lista del supermercado o una lista de pasos para una receta? En HTML tenemos **dos tipos de listas**:

#### Lista con viñetas (no ordenada)

Usa `<ul>` (*unordered list*) cuando el **orden no importa**, como una lista de ingredientes:

```html
<ul>
    <li>Color: gris</li>
    <li>Tamaño: 2 a 4 metros</li>
    <li>Hábitat: océanos</li>
</ul>
```

Esto se ve así:
- Color: gris
- Tamaño: 2 a 4 metros
- Hábitat: océanos

#### Lista numerada (ordenada)

Usa `<ol>` (*ordered list*) cuando el **orden sí importa**, como los pasos de una receta:

```html
<ol>
    <li>Busca una playa donde habiten delfines</li>
    <li>Lleva binoculares y observa con paciencia</li>
    <li>Mantén una distancia respetuosa</li>
</ol>
```

Esto se ve así:
1. Busca una playa donde habiten delfines
2. Lleva binoculares y observa con paciencia
3. Mantén una distancia respetuosa

> **Nota**: Cada elemento de la lista (ya sea `<ul>` o `<ol>`) va dentro de una etiqueta `<li>` (*list item*).

---

### ¿Cómo pongo imágenes?

Para mostrar una imagen usamos la etiqueta `<img>`. Esta etiqueta es especial porque **no tiene etiqueta de cierre** (no necesita `</img>`). Solo necesita dos atributos importantes:

| Atributo | ¿Para qué sirve? |
|----------|-------------------|
| `src`    | La **dirección** (URL) donde está la imagen |
| `alt`    | Un **texto alternativo** que describe la imagen (aparece si la imagen no carga y ayuda a personas con discapacidad visual) |

```html
<img src="https://ejemplo.com/delfin.jpg" alt="Un delfín saltando fuera del agua">
```

También puedes controlar el tamaño con el atributo `width` (ancho en píxeles):

```html
<img src="https://ejemplo.com/delfin.jpg" alt="Un delfín saltando" width="400">
```

> **Buena práctica**: Siempre incluye el atributo `alt`. Es como ponerle una etiqueta con nombre a una foto: si alguien no puede verla, la descripción le dice qué hay en ella.

---

### ¿Cómo creo enlaces (links)?

Los enlaces son lo que hace que la web sea una "red": te permiten **saltar de una página a otra** con un clic. Usamos la etiqueta `<a>` (*anchor*) con el atributo `href` que indica a dónde lleva el enlace.

```html
<a href="https://es.wikipedia.org/wiki/Delphinidae">Aprende más sobre delfines</a>
```

Si quieres que el enlace se abra en **una pestaña nueva** (sin salir de tu página), agrega `target="_blank"`:

```html
<a href="https://es.wikipedia.org/wiki/Delphinidae" target="_blank">
    Aprende más sobre delfines
</a>
```

Piensa en un enlace como una **puerta**: el texto que el usuario ve es el letrero de la puerta, y el `href` es el lugar al que lleva cuando la abres.

---

### ¿Cómo luce todo junto?

Así se ve el código que pegarías en el editor HTML de CodePen:

```html
<h1>El Delfín</h1>
<h2>Datos curiosos</h2>

<p>Los delfines son mamíferos marinos muy inteligentes.</p>
<p>Cada delfín tiene un silbido único, como su propio nombre.</p>

<ul>
    <li>Color: gris con el vientre claro</li>
    <li>Tamaño: entre 2 y 4 metros</li>
    <li>Hábitat: océanos de todo el mundo</li>
</ul>

<ol>
    <li>Busca una zona costera donde habiten delfines</li>
    <li>Lleva binoculares y observa con paciencia</li>
    <li>Mantén una distancia respetuosa</li>
</ol>

<img src="https://ejemplo.com/delfin.jpg" alt="Delfín saltando" width="400">

<a href="https://es.wikipedia.org/wiki/Delphinidae" target="_blank">
    Aprende más sobre los delfines
</a>
```

> **Nota sobre CodePen**: En CodePen solo escribes lo que va dentro del `<body>`. Las etiquetas `<!DOCTYPE>`, `<html>`, `<head>` y `<body>` ya las maneja CodePen por ti.

---

## Resumen rápido

| Elemento | Etiqueta | ¿Para qué sirve? |
|----------|----------|-------------------|
| Título principal | `<h1>` | El título más grande de la página |
| Subtítulos | `<h2>` a `<h6>` | Títulos secundarios, de mayor a menor |
| Párrafo | `<p>` | Bloques de texto normal |
| Lista con viñetas | `<ul>` + `<li>` | Lista donde el orden no importa |
| Lista numerada | `<ol>` + `<li>` | Lista donde el orden sí importa |
| Imagen | `<img>` | Muestra una foto (necesita `src` y `alt`) |
| Enlace | `<a>` | Crea un link a otra página (necesita `href`) |

---

## Actividad práctica

**Tu misión**: Crear una página sobre tu animal favorito que incluya:
1. Un título principal y un subtítulo
2. Dos párrafos con información interesante
3. Una lista con viñetas de sus características
4. Una lista numerada con pasos para observarlo o cuidarlo
5. Una imagen del animal
6. Un enlace a una página con más información