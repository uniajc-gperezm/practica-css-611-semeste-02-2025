# Práctica: CSS Grid Box

## ¿Qué es CSS Grid?
CSS Grid es un sistema de diseño bidimensional que permite crear layouts complejos y responsivos de manera sencilla utilizando filas y columnas. Con CSS Grid puedes posicionar elementos en una cuadrícula, controlar su tamaño y alineación, y crear estructuras flexibles para tus páginas web.

## Estructura de la Carpeta
- `index.html`: Archivo HTML principal que contiene la estructura de la cuadrícula y los elementos a posicionar.
- `css/styles.css`: Archivo de estilos donde se define y configura el grid y los estilos de los elementos.

## ¿Cómo funciona CSS Grid en este proyecto?
En el archivo `styles.css` se utiliza la clase `.grid-container` para definir el contenedor de la cuadrícula:

```css
.grid-container {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  grid-template-rows: repeat(2, 150px);
  gap: 10px;
  width: 600px;
}
```
- `display: grid;` activa el modo grid en el contenedor.
- `grid-template-columns: repeat(3, 1fr);` crea 3 columnas de igual tamaño.
- `grid-template-rows: repeat(2, 150px);` crea 2 filas de 150px de alto cada una.
- `gap: 10px;` agrega un espacio de 10px entre filas y columnas.

Cada elemento dentro del grid tiene una clase (`.a`, `.b`, `.c`, `.d`) que define su posición y color:

```css
.a {
  background-color: pink;
  grid-column: 1 / 3;
  grid-row: 1;
}

.b {
  background-color: lightblue;
  grid-column: 3 / 4;
  grid-row: 1 / 3;
}

.c {
  background-color: lightblue;
  grid-column: 1 / 2;
  grid-row: 2;
}

.d {
  background-color: lightgreen;
  grid-column: 2;
  grid-row: 2;
}
```
- `grid-column` y `grid-row` determinan la posición y el tamaño de cada caja dentro de la cuadrícula.

## Ventajas de CSS Grid
- Permite crear layouts complejos de forma sencilla.
- Facilita el diseño responsivo.
- El código es más limpio y fácil de mantener.

---

**Autor:** Generado con ayuda de AI (Copilot)

---

## Tips y Trucos para CSS Grid

- **Alineación avanzada:** Usa `justify-items`, `align-items`, `justify-content` y `align-content` para controlar la alineación de los elementos y la cuadrícula.
- **Áreas de grid:** Utiliza `grid-template-areas` para nombrar y organizar visualmente las zonas del grid, facilitando la lectura y el mantenimiento.
- **Grid implícito:** Si colocas más elementos de los definidos en el grid, CSS Grid creará filas o columnas adicionales automáticamente.
- **Fracciones (fr):** El valor `fr` permite repartir el espacio disponible de forma proporcional entre columnas o filas.
- **Minmax y auto-fill/auto-fit:** Usa `minmax()` junto con `auto-fill` o `auto-fit` para crear grids responsivos que se adapten al tamaño del contenedor.
- **Orden personalizado:** Puedes cambiar el orden visual de los elementos con la propiedad `order`.
- **Superposición de elementos:** Es posible superponer elementos usando la misma área de grid o ajustando `z-index`.
- **Combina con Flexbox:** Usa CSS Grid para el layout general y Flexbox para la alineación interna de los elementos.
- **Herramientas de inspección:** Usa las herramientas de desarrollo del navegador (DevTools) para visualizar y depurar la estructura del grid.

### Recursos para profundizar
- [Guía completa de CSS Grid en MDN](https://developer.mozilla.org/es/docs/Web/CSS/CSS_grid_layout)
- [CSS Tricks: A Complete Guide to Grid](https://css-tricks.com/snippets/css/complete-guide-grid/)
- [Grid by Example](https://gridbyexample.com/)

¡Experimenta y combina estas técnicas para crear layouts modernos y flexibles!

