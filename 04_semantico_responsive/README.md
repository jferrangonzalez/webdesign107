# Guía de Desarrollo Web: Etiquetas Semánticas HTML y Reglas Responsive CSS

Este documento proporciona una guía básica sobre el uso de etiquetas semánticas en HTML y la implementación de reglas responsive en CSS para crear sitios web accesibles, estructurados y adaptables a diferentes dispositivos.

---

## Etiquetas Semánticas HTML

Las etiquetas semánticas en HTML son aquellas que describen claramente el propósito de su contenido, mejorando la accesibilidad y el SEO del sitio web. A continuación, se presentan algunas de las etiquetas semánticas más comunes y su uso:

- **`<header>`**: Representa la cabecera de un documento o sección. Suele contener el logo, el título principal y la navegación.
- **`<nav>`**: Define un bloque de navegación, como menús o enlaces principales del sitio.
- **`<main>`**: Indica el contenido principal del documento, excluyendo encabezados, barras laterales y pies de página.
- **`<section>`**: Agrupa contenido relacionado dentro de una página, como secciones temáticas.
- **`<article>`**: Representa contenido independiente, como publicaciones de blog, artículos o noticias.
- **`<aside>`**: Contiene contenido relacionado o complementario, como barras laterales o widgets.
- **`<footer>`**: Define el pie de página de un documento o sección, que puede incluir información de contacto, derechos de autor o enlaces adicionales.
- **`<figure>` y `<figcaption>`**: Se utilizan para contenido visual (imágenes, gráficos, etc.) con una descripción o título asociado.
- **`<time>`**: Representa una fecha u hora específica, útil para eventos o publicaciones.

El uso de estas etiquetas mejora la estructura del documento, facilita la navegación para usuarios con tecnologías de asistencia y ayuda a los motores de búsqueda a comprender mejor el contenido.

---

## Reglas Responsive CSS

El diseño responsive permite que un sitio web se adapte a diferentes tamaños de pantalla y dispositivos, mejorando la experiencia del usuario. A continuación, se describen algunas técnicas y reglas clave para implementar CSS responsive:

### 1. **Uso de Media Queries**
Las media queries permiten aplicar estilos específicos según el ancho, la altura o la orientación de la pantalla. Ejemplo básico:
```css
/* Estilos para pantallas de hasta 768px */
@media screen and (max-width: 768px) {
    body {
        font-size: 14px;
    }
}

/* Estilos para pantallas de hasta 480px */
@media screen and (max-width: 480px) {
    body {
        font-size: 12px;
    }
}