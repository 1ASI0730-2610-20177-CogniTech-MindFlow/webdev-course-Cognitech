# Lección 5 — Proyecto Final: Crea tu página de perfil personal

**Duración estimada**: 15 minutos  
**Público**: Estudiantes de 12 a 17 años sin experiencia previa

---

## Contenido teórico

### ¿Cómo combinamos HTML y CSS en un mismo proyecto?

Hasta ahora usamos HTML para poner contenido (títulos, imágenes, listas) y CSS para darle color y estilo por separado.

En un proyecto real, ambos trabajan juntos al mismo tiempo.

HTML construye la estructura, como los pilares y paredes de una casa. CSS es la pintura, la decoración y los muebles que la hacen lucir bien.

Para unirlos, basta con escribir el HTML en una sección y el CSS en otra (como en CodePen), o usar la etiqueta `<style>` dentro del `<head>` de tu página.

El navegador lee ambos y los combina automáticamente para mostrarte el resultado final.

### ¿Cuáles son los errores más comunes al programar?

Todos los programadores, incluso los profesionales, cometen errores. Lo importante es saber reconocerlos y corregirlos.

Estos son los tres más frecuentes en HTML y CSS:

**1. Olvidarse de cerrar una etiqueta HTML**
Cada etiqueta que abres debe cerrarse. Si no lo haces, el navegador puede desordenar toda tu página sin avisar.

**2. Olvidarse del punto y coma en CSS**
En CSS, cada propiedad termina con `;`. Si lo olvidas, esa regla y las que siguen pueden fallar en silencio.

**3. No indentar el código**
Indentar significa dejar espacios para organizar visualmente el código. No afecta cómo funciona la página, pero hace que sea mucho más fácil de leer y corregir cuando algo falla.

### ¿Cómo luce el código?

Una página de perfil completa combina todo lo aprendido en el curso:

```html
<!DOCTYPE html>
<html>
  <head>
    <title>Mi Perfil Personal</title>
  </head>
  <body>

    <img src="https://i.pravatar.cc/150" alt="Mi foto de perfil">

    <h1>Hola, soy Ana García</h1>

    <p>Tengo 15 años y me encanta la música y el dibujo.</p>

    <h2>Mis hobbies favoritos:</h2>

    <ul>
      <li>Dibujar</li>
      <li>Escuchar música</li>
      <li>Leer libros</li>
    </ul>

    <a href="mailto:ana@correo.com">Contáctame</a>

  </body>
</html>
```

Y su CSS:

```css
body {
  background-color: #f0f4f8;
  font-family: Arial, sans-serif;
  text-align: center;
  padding: 40px;
}

img {
  width: 150px;
  border-radius: 50%;
  border: 4px solid #5c6bc0;
}

h1 {
  color: #3949ab;
  font-size: 28px;
}

h2 {
  color: #3949ab;
  font-size: 20px;
  margin-top: 24px;
}

p {
  color: #555;
  font-size: 16px;
}

ul {
  list-style: none;
  padding: 0;
  color: #555;
  font-size: 16px;
  line-height: 2;
}

a {
  background-color: #5c6bc0;
  color: white;
  padding: 10px 20px;
  text-decoration: none;
  border-radius: 8px;
  display: inline-block;
  margin-top: 20px;
}
```
