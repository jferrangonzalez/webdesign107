# README - Conceptos clave en HTML y CSS

## 1. ID y Clase

En HTML y CSS, **id** y **class** son atributos que permiten identificar y aplicar estilos a elementos específicos.

### **ID (`id`):**
- Es único en la página; no debe repetirse en otros elementos.
- Se usa con `#nombreID` en CSS.
- Ejemplo:
  ```html
  <div id="contenedor">Este es un contenedor</div>
  ```
  ```css
  #contenedor {
      background-color: lightblue;
  }
  ```

### **Clase (`class`):**
- Se puede aplicar a varios elementos.
- Se usa con `.nombreClase` en CSS.
- Ejemplo:
  ```html
  <p class="importante">Este es un texto importante.</p>
  ```
  ```css
  .importante {
      font-weight: bold;
      color: red;
  }
  ```

## 2. `font-family`

Define la fuente del texto en CSS. Se pueden establecer múltiples opciones en caso de que alguna no esté disponible.

- Ejemplo:
  ```css
  body {
      font-family: "Arial", "Helvetica", sans-serif;
  }
  ```
  - Si el sistema no tiene "Arial", usará "Helvetica".
  - Si tampoco tiene "Helvetica", usará cualquier fuente `sans-serif`.

## 3. `link`

Se usa en HTML para conectar el documento con archivos externos, como hojas de estilo CSS.

- Ejemplo de enlace a una hoja de estilos:
  ```html
  <link rel="stylesheet" href="estilos.css">
  ```
  - `rel="stylesheet"` indica que es una hoja de estilo.
  - `href="estilos.css"` especifica el archivo CSS a usar.

