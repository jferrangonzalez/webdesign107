# README.md

## Explicación de los conceptos de HTML y CSS utilizados

Este documento explica los conceptos fundamentales de HTML y CSS utilizados en la clase, incluyendo enlaces, selectores, propiedades CSS y efectos interactivos. El objetivo es proporcionar una guía clara y detallada para entender cómo se estructuran y estilizan las páginas web.

---

## **HTML: Estructura y Enlaces**

### **1. Tipos de Enlaces**
En HTML, los enlaces se crean con la etiqueta `<a>` y pueden tener diferentes propósitos según su uso:

- **Enlace a una página externa:**
  ```html
  <a href="https://www.google.es/" target="_blank">Ir a Google</a>
  ```
  - `href`: Define la URL del destino.
  - `target="_blank"`: Abre el enlace en una nueva pestaña.

- **Enlace a una página interna:**
  ```html
  <a href="index.html">INICIO</a>
  ```
  - Navega a otra página dentro del mismo proyecto.

- **Enlace a una sección específica de otra página:**
  ```html
  <a href="instrucciones.html#becas">CONDICIONES DE BECAS</a>
  ```
  - `#becas`: Indica el id del elemento al que se quiere dirigir.

- **Enlace a una sección dentro de la misma página:**
  ```html
  <a href="#zonacompras">Ir a comprar</a>
  ```
  - Navega a un elemento con el id `zonacompras` en la misma página.

- **Enlace para volver al inicio de la página:**
  ```html
  <a href="#contenedor">Ir arriba</a>
  ```

### **2. Listas con Enlaces**
Las listas se utilizan para organizar enlaces de manera estructurada:
```html
<ul class="navprincipal">
    <li><a href="index.html">INICIO</a></li>
    <li><a href="servicios.html">SERVICIOS</a></li>
    <li><a href="contacto.html">CONTACTO</a></li>
</ul>
```
- `<ul>`: Lista no ordenada.
- `<li>`: Elemento de la lista.
- `<a>`: Enlace dentro de cada elemento.

---

## **CSS: Estilización y Efectos Interactivos**

### **1. Reset Global**
El selector universal `*` se utiliza para eliminar márgenes y rellenos predeterminados de todos los elementos:
```css
* {
    padding: 0px;
    margin: 0px;
}
```

### **2. Estilización de Enlaces**
Se pueden aplicar estilos específicos a los enlaces dentro de una clase:
```css
.nav a {
    font-size: 30px;      /* Tamaño de fuente */
    margin-left: 10px;    /* Espaciado a la izquierda */
    color: red;           /* Color del texto */
}
```

### **3. Estilización de Listas**
Los elementos de lista pueden ser estilizados para parecer botones:
```css
.navprincipal li {
    list-style-type: none;    /* Elimina los marcadores de lista */
    width: 200px;             /* Ancho fijo */
    display: inline;          /* Elementos en línea */
    border: solid 1px red;    /* Borde rojo */
    padding: 5px 10px;        /* Espaciado interno */
    background: lightsalmon;  /* Color de fondo */
    border-radius: 4px;       /* Esquinas redondeadas */
}
```

### **4. Efectos Interactivos con `:hover`**
La pseudo-clase `:hover` permite aplicar estilos cuando el usuario pasa el cursor sobre un elemento:
```css
.navprincipal li:hover {
    border-radius: 9px;       /* Aumenta el redondeo de las esquinas */
    background: darkgreen;    /* Cambia el color de fondo */
    transition: 1s;           /* Transición suave de 1 segundo */
}
```

### **5. Estilización de Enlaces dentro de Listas**
Los enlaces dentro de los elementos de lista pueden tener estilos específicos:
```css
.navprincipal li a {
    color: white;             /* Color del texto */
    text-decoration: none;    /* Elimina el subrayado */
}
```

---

## **Resumen de Conceptos**

1. **HTML:**
   - Uso de enlaces para navegación interna, externa y dentro de la misma página.
   - Organización de enlaces en listas para crear menús de navegación.

2. **CSS:**
   - Reset global para un diseño uniforme.
   - Estilización de enlaces y listas para mejorar la apariencia.
   - Efectos interactivos con `:hover` para una mejor experiencia de usuario.

---

## **Cómo usar este proyecto**
1. **Estructura del proyecto:**
   - `index.html`: Página principal con enlaces y contenido.
   - `estilos.css`: Archivo CSS con las reglas de estilo.

2. **Subir a GitHub:**
   - Asegúrate de incluir ambos archivos en el repositorio.
   - Este archivo `README.md` proporciona una guía clara para entender el proyecto.

---

## **Licencia**
Este proyecto es de uso libre para fines educativos. Puedes modificarlo y adaptarlo según tus necesidades.