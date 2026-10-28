# Estándar de código del equipo

**Proyecto:** CorteFino
**Equipo:** desarrolladores
**Fecha:** 27 de octubre de 2026

Este documento es un acuerdo del equipo. Todas las personas lo siguen y se usa para revisar los pull requests.

## 1. HTML

- **H1.** El documento incluye doctype, `lang`, `meta charset`, `meta viewport` y un `title` con texto.
- **H2.** Etiquetas y atributos en minúsculas; valores entre comillas dobles.
- **H3.** Indentación de 2 espacios, sin tabulaciones.
- **H4.** Estructura semántica: `header`, `nav`, `main`, `section`, `article`, `footer`.
- **H5.** Un solo `h1` por página y encabezados en orden.
- **H6.** Toda imagen lleva `alt`.
- **H7.** Sin estilos en línea y sin `<br>` para espaciar.

## 2. CSS

- **C1.** El CSS vive en un archivo aparte (`css/style.css`).
- **C2.** Clases en kebab-case que dicen qué es, no cómo se ve.
- **C3.** Una propiedad por línea y un bloque por selector.
- **C4.** Colores y medidas repetidas en variables dentro de `:root`.
- **C5.** Sin `!important` ni selectores por id para dar estilo.
- **C6.** Diseño adaptable: unidades relativas, flex o grid, `max-width` en lugar de anchos fijos.

## 3. Nuestras reglas propias

1. **Nombres de imágenes.** Las imágenes van en `img/` y su nombre dice qué muestran, con el tamaño si aplica: `agua-600ml.jpg`, no `foto1.jpg`.
2. **Orden de las propiedades CSS.** Primero layout (`display`, `grid-template-columns`, `gap`, `max-width`), luego caja (`margin`, `padding`, `border`), luego tipografía (`font-*`) y al final color y efectos (`color`, `background`, `cursor`).
3. **Comentarios.** El CSS se divide en secciones con un comentario en minúscula (`/* === tarjetas === */`) y en el HTML se comenta el inicio de cada bloque grande (`<!-- productos -->`).

## 4. Archivos, ramas y commits

- Carpetas y archivos: minúsculas con guiones, sin espacios ni tildes (`css/`, `js/`, `img/`).
- Ramas: `feature/`, `fix/` o `docs/` seguido de una descripción corta. Ejemplo: `docs/estandar`.
- Commits: en presente, que expliquen qué se hizo. Ejemplo: `Agrega alt a las imágenes (H6)`.

## 5. Base de datos

- Tablas: plural y en snake_case (`detalle_pedido`).
- Columnas: snake_case. Claves foráneas con el nombre de la tabla en singular y `_id` (`cliente_id`).
- Palabras clave de SQL en MAYÚSCULAS.

## 6. Cómo lo verificamos

- **Herramientas:** validador HTML del W3C (validator.w3.org), validador CSS del W3C (jigsaw.w3.org/css-validator) y modo responsive de las herramientas del navegador (F12) probando con 360 px de ancho.
- **Quién revisa cada pull request:** otro integrante del equipo, usando la tabla de revisión. Nadie aprueba su propio pull request.
- **Qué pasa si una regla no se cumple:** el revisor marca "Pide cambios antes de unir a main", quien hizo el PR corrige en la misma rama y vuelve a pedir revisión. No se une a `main` hasta que quede aprobado.

## Firmas del equipo

- Jesús Castro
