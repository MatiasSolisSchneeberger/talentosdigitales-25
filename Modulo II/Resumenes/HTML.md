# Apunte de Estudio: HTML 
## Introducción al HTML-Tema1-parte 1

### ¿Qué es HTML?
HTML (**HyperText Markup Language**): Lenguaje de marcado para crear páginas web.

Define la estructura y contenido de una página (texto, imágenes, enlaces, etc.).

No es un lenguaje de programación, sino una forma de organizar información para navegadores.

### Historia y Evolución
Creado en 1991 por Tim Berners-Lee con fines divulgativos.

HTML5 es el estándar actual, gestionado por el W3C (World Wide Web Consortium).

Evolucionó para cubrir necesidades multimedia y semánticas.

### Estructura Básica de un Documento
**Etiquetas**: Elementos entre `< >` que definen contenido.

Ejemplo: `<p>Texto</p>` (párrafo), `<strong>Texto</strong>` (importancia semántica).

Elementos vacíos: No requieren cierre (ejemplo: `<img src="imagen.jpg" alt="Descripción">`).

**Atributos**: Modifican el comportamiento de las etiquetas.

Ejemplo: `<a href="https://ejemplo.com">Enlace</a>`.

### Etiquetas y Atributos Comunes
Etiquetas básicas:

- `<h1> a <h6>`: Encabezados.

- `<a>`: Enlaces.

- `<img>`: Imágenes.

- `<ul>, <ol>, <li>`: Listas.

Atributos clave:

**id**: Identificador único (ejemplo: `<div id="header">`).

**class**: Clases reutilizables (ejemplo: `<div class="menu">`).

**style**: Estilos CSS en línea (evitar su uso excesivo).

### Semántica en HTML5
Objetivo: Separar contenido (HTML) de presentación (CSS).

Etiquetas semánticas:

`<header>`, `<footer>`, `<article>`, `<section>`, `<nav>`.

Ejemplo:

Usar `<strong>` (importancia semántica) en lugar de `<b>` (negrita visual).

### Herramientas Recomendadas
Editores de texto: _VS Code_, _Sublime Text_, _Notepad++_.

Entornos online:
- **CodePen**: Ideal para pruebas rápidas de HTML/CSS/JS.
- **CodeSandbox**: Desarrollo web colaborativo con integración a GitHub.

### Mejores Prácticas
Validar código: Usar herramientas como el Validador del W3C.

Comentarios: Documentar con `<!-- Esto es un comentario -->`.

Evitar estilos en línea: Usar CSS externo para mantener separación de responsabilidades.

### Ejemplo de Código Básico

```html
<!DOCTYPE html>
<html lang="es">
    <head>
        <title>Mi Primera Página</title>
    </head>
    <body>
        <header>
            <h1>Bienvenido</h1>
        </header>
        <main>
            <p>Este es un <strong>párrafo importante</strong>.</p>
            <img src="logo.png" alt="Logo">
        </main>
    </body>
</html>
```

---

## Apunte de Estudio: Introducción a HTML (Tema 1 - Parte 2)

## Estructura Básica de un Documento HTML
`<!DOCTYPE html>`: Declaración inicial para indicar que el documento sigue el estándar HTML5.

Elementos esenciales:

```html
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <title>Título de la página</title>
</head>
<body>
    <!-- Contenido visible -->
</body>
</html>
```

`<meta charset="UTF-8">`: Define la codificación de caracteres (UTF-8 recomendado).

## Recomendaciones Prácticas
**Nombres de archivos:**

Evitar espacios, acentos y caracteres especiales.

Usar guiones (`-`) o guiones bajos (`_`). Ejemplo: `quienes_somos.html`.

**Visualización en navegadores:**

Verificar la página en múltiples navegadores (Chrome, Firefox, Edge).

Acceder al código fuente con **Ctrl+U** o Inspeccionar elemento (botón derecho).

## Formato de Texto y Párrafos
**Etiquetas básicas:**

`<p>`: Define un párrafo (agrega espacio antes y después).

`<br>`: Salto de línea sin espacio (no requiere cierre).

**Advertencia:**

Evitar el atributo align (ejemplo: `<p align="center">`) por estar obsoleto en HTML. Usar CSS para estilos.

## Encabezados Semánticos
**Jerarquía de encabezados:**

```html
<h1>Título principal</h1> <!-- Nivel 1 (más importante) -->
<h2>Subtítulo</h2>       <!-- Nivel 2 -->
<h3>Sub-subtítulo</h3>   <!-- Nivel 3 -->
<!-- ... hasta h6 -->
 ```

**Propósito:** Estructurar el contenido, no solo cambiar el tamaño del texto.

**Semántica:** Ayuda a motores de búsqueda (SEO) y accesibilidad.

## Ejemplo de Página Completa
```html
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <title>Encabezados</title>
</head>
<body>
    <h1>Encabezado nivel 1</h1>
    <h2 align="center">Encabezado nivel 2 (alineado al centro)</h2>
    <div>
        <p>Párrafo alineado a la izquierda.</p>
        <p>Otro párrafo.</p>
    </div>
    <br><br><br> <!-- Saltos de línea -->
    <p>Texto final.</p>
</body>
</html>
```

## Buenas Prácticas
**Separación de responsabilidades:**

- HTML para contenido.

- CSS para estilos visuales.

**Validación:** Usar herramientas como el Validador del W3C.