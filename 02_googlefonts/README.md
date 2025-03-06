# README.md

## Explicación de los conceptos de Google Fonts y Colores Web

Este documento explica los conceptos fundamentales de Google Fonts y Colores Web utilizados en el proyecto, incluyendo la integración de fuentes, propiedades CSS y técnicas de aplicación de colores. El objetivo es proporcionar una guía clara y detallada para entender cómo se implementan estos elementos en páginas web.

---

## **Google Fonts: Integración y Uso**

### **1. Configuración en el HTML**
Para integrar Google Fonts en un proyecto web, se deben incluir los siguientes elementos en la sección `<head>`:

- **Preconexión a servidores:**
  ```html
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  ```
  - `preconnect`: Establece conexión anticipada para mejorar el rendimiento.
  - `crossorigin`: Habilita el uso de CORS para recursos externos.

- **Carga de fuentes específicas:**
  ```html
  <link href="https://fonts.googleapis.com/css2?family=Nunito+Sans:ital,opsz,wght@0,6..12,200..1000;1,6..12,200..1000&family=Yellowtail&display=swap" rel="stylesheet">
  ```
  - Carga las fuentes Nunito Sans (con múltiples variaciones) y Yellowtail.
  - El parámetro `display=swap` muestra texto con fuente alternativa mientras se cargan las fuentes de Google.

### **2. Implementación en CSS**
Las fuentes cargadas se aplican a elementos específicos mediante CSS:

- **Fuente principal para el cuerpo:**
  ```css
  body {
      font-family: "Nunito Sans", sans-serif;
      font-optical-sizing: auto;
      font-weight: 400;
      font-style: normal;
      font-variation-settings:
        "wdth" 100,
        "YTLC" 500;
  }
  ```
  - `font-family`: Define la fuente principal con alternativa sans-serif.
  - `font-optical-sizing`: Ajusta automáticamente el diseño óptico según el tamaño.
  - `font-variation-settings`: Configura características específicas de fuentes variables.

- **Fuente decorativa para encabezados:**
  ```css
  h1, h2, h3 {
      font-family: "Yellowtail", cursive;
      font-weight: 400;
      font-style: normal;
      color: #ff0000;
  }
  ```
  - Aplica la fuente Yellowtail a todos los encabezados con alternativa cursive.

---

## **Colores Web: Formatos y Aplicación**

### **1. Formatos de Color en CSS**
CSS permite definir colores de diferentes maneras:

- **Colores por nombre:**
  ```css
  background-color: cornsilk;
  ```
  - Utiliza nombres predefinidos en CSS para colores específicos.

- **Colores hexadecimales:**
  ```css
  color: #ff0000;
  ```
  - Formato de 6 dígitos que representa valores RGB en base 16.
  - `#ff0000` corresponde al color rojo puro.

- **Colores RGBA:**
  ```css
  background-color: rgba(24, 197, 240, 0.137);
  ```
  - Formato que incluye canal alfa (transparencia).
  - Los valores RGB van de 0 a 255, y el alfa de 0 (transparente) a 1 (opaco).

### **2. Aplicación de Colores**
Los colores se aplican a diferentes elementos para crear la apariencia visual:

- **Fondo de secciones:**
  ```css
  .text-hero {
      background-color: cornsilk;
      height: 100vh;
  }
  ```
  - Aplica un color de fondo amarillo pálido a la sección principal.

- **Colores de texto:**
  ```css
  h1, h2, h3 {
      color: #ff0000;
  }
  ```
  - Define el color rojo para todos los textos de encabezado.

- **Fondos con transparencia:**
  ```css
  .encabezado {
      text-align: center;
      background-color: rgba(24, 197, 240, 0.137);
  }
  ```
  - Crea un fondo azul claro semi-transparente para el contenedor de encabezados.

---

## **Diseño Responsive y Layout**

### **1. Configuración del Viewport**
Para garantizar que el diseño se adapte a diferentes dispositivos:

```html
<meta name="viewport" content="width=device-width, initial-scale=1.0">
```
- `width=device-width`: Ajusta el ancho al tamaño del dispositivo.
- `initial-scale=1.0`: Establece el nivel de zoom inicial.

### **2. Técnicas de Layout**
Se utilizan técnicas modernas para estructurar el contenido:

- **CSS Grid para centrado:**
  ```css
  .text-hero {
      display: grid;
      align-items: center;
  }
  ```
  - Centra verticalmente el contenido dentro de la sección hero.

- **Altura adaptativa:**
  ```css
  .text-hero {
      height: 100vh;
  }
  ```
  - Hace que la sección ocupe el 100% de la altura visible del navegador.

- **Centrado de texto:**
  ```css
  .encabezado {
      text-align: center;
  }
  ```
  - Alinea el texto al centro horizontalmente.

---

## **Mejores Prácticas Implementadas**

### **1. Reset CSS**
```css
* {
    padding: 0px;
    margin: 0px;
}
```
- Elimina márgenes y rellenos predeterminados para mayor control del diseño.

### **2. Fuentes Alternativas**
```css
font-family: "Nunito Sans", sans-serif;
font-family: "Yellowtail", cursive;
```
- Proporciona fuentes genéricas como respaldo en caso de fallo en la carga.

### **3. Estructura Semántica**
```html
<div id="contenedor">
    <div class="text-hero">
        <div class="encabezado">
            <h1>Mujeres que cambiaron tu historia.</h1>
            <h2>Lee y aprende</h2>
        </div>
    </div>
</div>
```
- Organiza el contenido en contenedores lógicos con nombres descriptivos.
