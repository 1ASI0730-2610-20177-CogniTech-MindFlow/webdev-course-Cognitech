# Lección 2 — HTML básico: etiquetas, elementos y atributos

**Duración estimada**: 12 minutos  
**Público**: Estudiantes de 12 a 17 años sin experiencia previa

---

# Contenido teórico

## ¿Qué es HTML?

HTML significa HyperText Markup Language o Lenguaje de Marcado de Hipertexto.

Es el lenguaje utilizado para construir la estructura de una página web. Si imaginamos una página web como una casa, HTML sería el esqueleto o la estructura que sostiene todos los elementos.

HTML no se utiliza para agregar colores o animaciones. Su función principal es organizar la información que aparecerá en pantalla.

---

## ¿Cómo interpreta HTML el navegador?

Cuando escribimos código HTML, el navegador lee las instrucciones y las transforma en una página visual.

Por ejemplo, si escribimos:

```html
<h1>Bienvenidos</h1>
```

el navegador mostrará:

# Bienvenidos

Es decir, HTML no se muestra como texto plano, sino que el navegador interpreta las etiquetas y genera el contenido visual.

---

## ¿Qué es una etiqueta HTML?

Las etiquetas son instrucciones que indican al navegador cómo debe interpretar el contenido.

La mayoría de etiquetas tienen una apertura y un cierre.

```html
<h1>Mi primera página web</h1>
```

La etiqueta de apertura es:

```html
<h1>
```

La etiqueta de cierre es:

```html
</h1>
```

Todo lo que se encuentra entre ambas etiquetas corresponde al contenido.

---

## Anatomía de una etiqueta

Observemos el siguiente ejemplo:

```html
<p>Estoy aprendiendo HTML.</p>
```

Está compuesto por:

- Etiqueta de apertura:

```html
<p>
```

- Contenido:

```text
Estoy aprendiendo HTML.
```

- Etiqueta de cierre:

```html
</p>
```

Las etiquetas de cierre se diferencian porque contienen una barra inclinada (/).

---

## ¿Qué es un elemento HTML?

Un elemento HTML está formado por:

1. La etiqueta de apertura.
2. El contenido.
3. La etiqueta de cierre.

Por ejemplo:

```html
<p>Este es un párrafo.</p>
```

Todo el conjunto representa un elemento HTML.

De igual manera:

```html
<h1>Mi sitio web</h1>
```

es otro elemento HTML.

---

## Elementos anidados

Los elementos HTML pueden contener otros elementos.

Por ejemplo:

```html
<body>

    <h1>Mi página web</h1>

    <p>Bienvenidos al curso de desarrollo web.</p>

</body>
```

En este caso:

- `<body>` es el elemento padre.
- `<h1>` y `<p>` son elementos hijos.

La anidación permite organizar mejor la información.

---

## ¿Qué son los atributos?

Los atributos proporcionan información adicional sobre una etiqueta.

Se escriben dentro de la etiqueta de apertura.

Su estructura es:

```html
nombre="valor"
```

Ejemplo:

```html
<a href="https://www.google.com">
    Ir a Google
</a>
```

Aquí:

- `<a>` crea un enlace.
- `href` es un atributo.
- `"https://www.google.com"` es el valor del atributo.

---

## Estructura general de un atributo

```html
<etiqueta atributo="valor">
```

Ejemplo:

```html
<img src="foto.jpg">
```

En este caso:

- `src` es el atributo.
- `"foto.jpg"` es su valor.

Los atributos permiten personalizar el comportamiento de las etiquetas.

---

## ¿Por qué son importantes los atributos?

Los atributos permiten:

- Definir direcciones web.
- Identificar elementos.
- Agregar información adicional.
- Personalizar características específicas.

Por ejemplo:

```html
<a href="https://www.wikipedia.org">
    Visitar Wikipedia
</a>
```

Sin el atributo `href`, el enlace no sabría hacia dónde dirigirse.

---

## Estructura básica de un documento HTML

Toda página web comienza con una estructura similar:

```html
<!DOCTYPE html>
<html>

<head>

    <title>Mi primera página</title>

</head>

<body>

</body>

</html>
```

---

## ¿Qué función cumple cada parte?

### <!DOCTYPE html>

Indica que el documento utiliza HTML5.

```html
<!DOCTYPE html>
```

---

### html

Representa el documento completo.

```html
<html>

</html>
```

---

### head

Contiene información interna que no se muestra directamente al usuario.

```html
<head>

</head>
```

---

### title

Define el nombre que aparece en la pestaña del navegador.

```html
<title>Mi primera página</title>
```

---

### body

Contiene todo lo visible de la página.

```html
<body>

</body>
```

Dentro del body se colocarán los elementos que veremos en la siguiente lección.

---

## Resumen

En esta lección aprendimos:

✓ Qué es HTML.

✓ Cómo interpreta HTML el navegador.

✓ Qué son las etiquetas.

✓ Qué es un elemento HTML.

✓ Qué significa la anidación de elementos.

✓ Qué son los atributos.

✓ La estructura básica de una página HTML.

En la siguiente lección aprenderemos a utilizar elementos HTML comunes como títulos, párrafos, listas, imágenes y enlaces.
