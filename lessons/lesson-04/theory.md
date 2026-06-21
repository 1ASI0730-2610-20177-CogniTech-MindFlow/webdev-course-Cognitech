# Lección 4 — Introducción a CSS: colores, fuentes, selectores y bordes

**Duración estimada**: 6 minutos  
**Público**: Estudiantes de 12 a 17 años sin experiencia previa

---

## Contenido teórico

En las lecciones anteriores construimos el "esqueleto" de nuestra página web usando HTML. Pusimos textos, listas y fotos, pero seamos sinceros: se ve un poco aburrida, ¿verdad? ¡Es hora de darle vida!

Aquí es donde entra **CSS** (Hojas de Estilo en Cascada). Si HTML es el cuerpo y los huesos de una página, CSS es la ropa, el peinado, los colores y el estilo. CSS convierte un documento de texto simple en un sitio web moderno, colorido y atractivo.

---

### ¿Cómo le doy órdenes a CSS? (La Regla Mágica)

Para cambiar el estilo de algo, necesitamos aprender a darle instrucciones al navegador. En CSS, siempre usamos una regla que tiene tres partes clave:

1. **El Selector**: ¿A *quién* le vamos a cambiar el estilo? (ej. a todos los párrafos `<p>`, o a todo el cuerpo `<body`>).
2. **La Propiedad**: ¿*Qué* le vamos a cambiar? (ej. el color, el tamaño).
3. **El Valor**: ¿*Cómo* va a quedar? (ej. azul, grande).

```css
selector {
    propiedad: valor;
}
```
Regla de oro de CSS: Siempre abrimos y cerramos nuestras reglas con llaves `{ }` y terminamos cada instrucción con un punto y coma `;`. Si olvidas el punto y coma, ¡el navegador se confunde y los estilos se rompen!

### ¿Cómo pinto mi página? (Colores)
Podemos cambiar los colores de dos cosas principalmente: el texto y el fondo.

1. **color**: Cambia el color de la letra.
2. **background-color**: Cambia el color del fondo (la pared detrás de tu texto).

Puedes usar los nombres de los colores en inglés (como red, blue, black, orange).

```css
/* Cambiamos el color de fondo de TODA la página */
body {
    background-color: lightblue;
}

/* Hacemos que el título principal sea de color blanco */
h1 {
    color: white;
}
```

### ¿Cómo cambio la letra? (Fuentes)
Las páginas con la letra que viene por defecto a veces se ven como documentos muy antiguos. Vamos a modernizarlas cambiando el tipo de fuente y el tamaño.

1. **font-family**: Cambia el tipo de letra (tipografía).
2. **font-size**: Cambia el tamaño de la letra. En la web usamos px (píxeles) para medirla.
```css
p {
    font-family: Arial, sans-serif;
    font-size: 18px;
}
```
Piensa en font-family como elegir tu letra favorita en Word, y en font-size como el numerito del tamaño.

### ¿Cómo pongo marcos y fotos redondas? (Bordes)
¿Has notado que en Instagram o TikTok tu foto de perfil es un círculo perfecto? ¡Eso se hace con CSS!

1. **border**: Dibuja un marco alrededor de tu elemento. Necesita tres valores juntos: el grosor, el estilo de la línea y el color. (ej. 5px solid black).
2. **border-radius**: Redondea las esquinas de los elementos.
```css
img {
    border: 5px solid gray;
    border-radius: 50%;
}
```
El truco mágico del 50%: Si a cualquier imagen cuadrada le pones la propiedad border-radius: 50%;, ¡se convertirá automáticamente en un círculo perfecto!

## ¿Cómo luce todo junto?
Imagina que tienes este HTML en tu página web:
```html
<h1>Mi Perfil Personal</h1>
<img src="[https://ejemplo.com/mifoto.jpg](https://ejemplo.com/mifoto.jpg)" alt="Mi foto de perfil">
<p>¡Hola! Me encanta aprender a diseñar páginas web.</p>
```
Para que se vea increíble, este sería el código que escribirías en la pestaña de CSS en CodePen:
```css
/* Pintamos el fondo de gris oscuro y cambiamos la letra de todo */
body {
    background-color: #333333;
    font-family: Arial, sans-serif;
}
/* Título centrado y de color amarillo brillante */
h1 {
    color: yellow;
    text-align: center; /* Esto centra el texto en medio de la pantalla */
}
/* Párrafo con letra más grande y color blanco */
p {
    font-size: 20px;
    color: white;
}
/* Imagen redonda y con un marco amarillo que hace juego */
img {
    border: 5px solid yellow;
    border-radius: 50%;
}
```

## Resumen rápido

| Propiedad CSS | ¿Para qué sirve? | Ejemplo de uso |
|----------|----------|-------------------|
| `color` | Cambia el color del texto | `color: red;` |
| `background-color` | Cambia el color del fondo | `background-color: black;` |
| `font-family` | Cambia el tipo de letra | `font-family: Arial;` |
| `font-size` | Cambia el tamaño de la letra | `font-size: 24px;` |
| `text-align` | Alinea el texto (izquierda, derecha, centro) | `text-align: center;` |
| `border` | Dibuja un marco alrededor del elemento | `border: 2px solid blue;` |
| `border-radius` | Redondea las esquinas (50% hace un círculo) |  `border-radius: 50%;` |

## Actividad práctica
¡Es hora de convertirte en diseñador! Entra a CodePen y usa el HTML que creaste en la lección anterior.

Tu misión en el panel de CSS:
1. Usa el selector body para pintar el fondo de tu página de tu color favorito (¡recuerda escribirlo en inglés!).
2. Cambia el color (color) y el tipo de letra (font-family) de tu título `<h1>` .
3. Haz que el texto de tus párrafos sea más fácil de leer haciéndolo más grande usando font-size.
4. ¡El toque maestro! Haz que la imagen de tu página destaque poniéndole un marco (border) y convirtiéndola en un círculo perfecto usando border-radius: 50%;.