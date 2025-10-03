# Práctica: Metodología BEM

## ¿Qué es BEM?
BEM (Bloque, Elemento, Modificador) es una metodología para nombrar clases CSS que ayuda a escribir código más estructurado, reutilizable y fácil de mantener. BEM divide la interfaz en bloques independientes, sus elementos internos y posibles variaciones (modificadores).

- **Bloque**: Una entidad independiente que representa un componente funcional (por ejemplo, `card`, `boton`, `frase`).
- **Elemento**: Una parte de un bloque que no tiene sentido fuera de él. Se nombra usando el bloque seguido de dos guiones bajos y el nombre del elemento (por ejemplo, `card__titulo`, `boton__icono`).
- **Modificador**: Una variante o estado de un bloque o elemento. Se nombra usando el bloque o elemento seguido de dos guiones y el nombre del modificador (por ejemplo, `boton--verde`, `boton--absolute`).

## Estructura del Código en esta Carpeta

- `index.html`: Contiene la estructura HTML usando clases con la convención BEM. Ejemplo:
  - `<div class="card">` es un **bloque**.
  - `<h3 class="card__titulo">` es un **elemento** del bloque `card`.
  - `<a class="boton boton--verde">` es un **bloque** con un **modificador**.

- `css/styles.css`: Define los estilos para los bloques, elementos y modificadores siguiendo la nomenclatura BEM.

- `images/`: Carpeta de imágenes usadas en la práctica.

## Ejemplo de BEM en el código
```html
<div class="card"> <!-- Bloque -->
  <a href="#" class="card__thumbnail">
    <img class="card__img" src="images/1.jpg" alt="">
  </a>
  <div class="card__textos">
    <h3 class="card__titulo">
      <a href="#" class="card__enlace">Título</a>
    </h3>
    <p class="card__extracto">Extracto de la tarjeta.</p>
    <a href="#" class="boton boton--verde">
      <span class="boton__texto">Ver Más</span>
      <i class="boton__icono fas fa-arrow-right"></i>
    </a>
  </div>
</div>
```

## Ventajas de BEM
- Facilita la lectura y mantenimiento del código.
- Evita conflictos de nombres en CSS.
- Permite reutilizar componentes y estilos.

---

**Autor:** Generado con ayuda de AI (Copilot)
