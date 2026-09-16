# Tarea 1

Tarea del curso SOFT-12-C1 -- Programación Web Avanzada

**Estudiante:** Sidney Rodríguez

**Seccion:** SCV2   **Periodo:** III Cuatrimestre 2026

**Docente:** Álvaro Cordero Peña

## Descripción

Desarrollo de dos casos prácticos independientes orientados a la construcción de interfaces web accesibles y adaptables utilizando HTML5 y CSS3.

## Estructura del repositorio

- `Tarea1/` — carpeta principal del repositorio
  - `caso1/` — archivos, estilos y recursos del primer caso
    - `index.html` — página principal del caso 1
    - `css/` — carpeta de hojas de estilo
      - `estilos.css` — estilos personalizados para el caso 1
    - `img/` — recursos gráficos e imágenes del caso 1
  - `caso2/` — archivos, estilos y recursos del segundo caso
    - `index.html` — página principal del caso 2
    - `css/` — carpeta de hojas de estilo
      - `estilos.css` — estilos personalizados para el caso 2
    - `img/` — recursos gráficos e imágenes del caso 2
 
## Cómo ejecutar
 
Abrir `caso1/index.html` o `caso2/index.html` en el navegador. No requiere instalación.

## Decisiones de diseño
 
### Caso 1:
Selección de etiquetas semánticas
En lugar de usar muchos div, se estructuró el HTML con etiquetas semánticas (<main>, <section>, <article>, <aside>) para darle un sentido lógico al contenido. Se mantuvo una jerarquía de usar solo un <h1> para el título del sitio, <h2> para separar las secciones y <h3> para los títulos dentro de las tarjetas, como se vió en clase.

Accesibilidad
Se agrega lang="es", se conectan las secciones con sus respectivos títulos usando aria-labelledby, y se utilizaron atributos alt para las descripciones de las imágenes en la galería. Además, los estados de las misiones, por ejemplo, incluyen texto explícito (ejemplo: "En progreso") para no depender solo de colores.

Modelo de caja y cascada CSS
Se utiliza box-sizing: border-box de forma global para que los bordes y rellenos no se desborden. Se mantiene la especificidad del CSS baja utilizando "class" y no se utiliza "!important". Para las separaciones, se utiliza gap en la mayoría de las ocasiones, en vez de márgenes fijos.

Posicionamiento
Se utiliza position: sticky en el header, porque permite que el nombre de la expedición y el menú de navegación queden fijos mientras el usuario hace scroll para leer todas las secciones.

Grid y Flexbox
Se utiliza felxbox para alinear elementos en una sola dirección, como el menú de navegación, la lista de la agenda y para los textos que van dentro de las tarjetas.
Se usó CSS Grid para la estructura general bidimensional, como para separar el área principal de la columna lateral ""grid-template-columns: minmax(0, 1fr) 18rem;" y crear las cuadrículas de las tarjetas paera que mantengan la misma altura.

Mobile-First y Media Queries
El CSS se inicia pensando en cómo se debe ver la página desde un celular, luego se usan dos media queries a partir de 48rem y 64rem para reorganizar el layout y aprovechar el espacio más ancho

Variables y unidades relativas
Se evita el uso de pixeles como medida, pues es estático y podría causar problemas para adaptarse a diferentes pantallas. Se emplea principalmente rem para fuentes y espaciados, y % y fr para hacer las cajas. Además, se centraliza la paleta de colores y los espacios en el bloque :root con variables CSS, lo cual ayuda a mantener la consistencia del diseño de la página.
 
## Resumen de commits

| # | Fecha | Hash | Mensaje | Zona | Cambio |
|---|---|---|---|---|---|
| 1 | 2026-09-08 | b41614f | Creación de la estructura base del repositorio | Global | Carpetas |
| 2 | 2026-09-11 | d2fd141 | Avance de caso 1 - html:  header, resumen de operaciones, misiones activas | caso1 | caso1/index.html |
| 3 | 2026-09-13 | 1bd03c8 | Cambios en html y configuración inicial css de caso 1  | caso1 | caso1/index.html y caso1/css/estilos.css |
| 4 | 2026-09-13 | 44a6fa4 | Actualización CSS: Header y contenedores principales + Actualización de tabla de commits | caso1 | caso1/index.html y caso1/css/estilos.css
| 5 | 2026-09-13 | 3c19b5c | Actualización CSS y HTML: Resumen de operaciones y Misiones activas | caso1 | caso1/index.html y caso1/css/estilos.css
| 6 | 2026-09-14 | 335833f | Actualización CSS y HTML: Equipos operativos | caso1 | caso1/index.html y caso1/css/estilos.css
| 7 | 2026-09-15 | 2d8adc7 | Actualizaciones y correcciones HTML y CSS | caso1 | caso1/index.html y caso1/css/estilos.css
| 8 | 2026-09-15 | e0cb0cb | Se agregan las imágenes a la carpeta img del caso 1 y se edita el html | caso1 | caso1/index.html y caso1/img
