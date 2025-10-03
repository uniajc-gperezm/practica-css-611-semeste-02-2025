# Práctica: Cards Layout con clip-path

## Descripción del Proyecto
Esta carpeta contiene un ejemplo de tarjeta de perfil (Profile Card) con un diseño moderno utilizando la propiedad CSS `clip-path` para crear formas personalizadas en los encabezados y pies de la tarjeta.

## Estructura de la Carpeta
- `index.html`: Contiene la estructura HTML de la tarjeta de perfil.
- `css/styles.css`: Archivo de estilos donde se aplican los efectos visuales con `clip-path` y otros estilos.

## ¿Cómo funciona la propiedad clip-path?
La propiedad `clip-path` en CSS permite recortar ("clippear") el área visible de un elemento, mostrando solo la parte que queda dentro de la forma definida. Es muy útil para crear efectos visuales avanzados y formas no rectangulares sin necesidad de imágenes adicionales o SVGs.

### Sintaxis básica
```css
clip-path: <forma>;
```
Donde `<forma>` puede ser un círculo, elipse, inset, path o un polígono.

## ¿Cómo funciona el valor polygon en clip-path?
El valor `polygon` permite definir una forma personalizada usando una lista de puntos (coordenadas X e Y) que forman los vértices del polígono. Cada punto se expresa como un porcentaje relativo al ancho y alto del elemento.

### Ejemplo:
```css
clip-path: polygon(0% 0%, 100% 0%, 100% 86%, 66% 75%, 50% 59%, 35% 75%, 0 86%);
```
- Cada par de valores representa un vértice del polígono.
- El primer valor es el porcentaje horizontal (X), el segundo es el vertical (Y).
- Los puntos se conectan en orden y el último punto se conecta con el primero para cerrar la figura.

En este proyecto, se usa `clip-path: polygon(...)` para dar formas originales al header y al footer de la tarjeta, logrando un diseño atractivo y moderno.

## ¿Cómo funciona un CDN?
Un CDN (Content Delivery Network) es una red de servidores distribuidos geográficamente que permite entregar archivos estáticos (como imágenes, hojas de estilo, scripts o fuentes) de manera rápida y eficiente. Al usar un CDN, los recursos se descargan desde el servidor más cercano al usuario, mejorando la velocidad de carga y el rendimiento del sitio web.

### Ventajas de usar un CDN
- Reducción del tiempo de carga.
- Menor consumo de ancho de banda del servidor principal.
- Mayor disponibilidad y redundancia.
- Mejor experiencia de usuario a nivel global.

## ¿Cómo usamos Font Awesome para los iconos?
[Font Awesome](https://fontawesome.com/) es una biblioteca de iconos vectoriales que se integra fácilmente en proyectos web. Se puede usar mediante un CDN, agregando un enlace `<link>` en el `<head>` del HTML. Luego, los iconos se insertan usando etiquetas `<i>` con clases específicas.

### Ejemplo de uso en este proyecto
```html
<!-- Enlazamos el CDN de Font Awesome en el head -->
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">

<!-- Usamos los iconos en el HTML -->
<i class="fas fa-plus"></i>
<i class="fab fa-facebook"></i>
```
- `fas` indica un icono sólido, `fab` un icono de marca.
- El nombre del icono (por ejemplo, `fa-plus`, `fa-facebook`) determina el símbolo que se muestra.

Font Awesome permite personalizar el tamaño, color y animación de los iconos fácilmente con CSS.

## Recursos útiles
- [Editor visual de clip-path (Clippy)](https://bennettfeely.com/clippy/)
- [Guía de clip-path en MDN](https://developer.mozilla.org/es/docs/Web/CSS/clip-path)

---

**Autor:** Generado con ayuda de AI (Copilot)


