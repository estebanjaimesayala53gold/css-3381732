# Catálogo Web de Dulcería Artesanal - Dulcería Goldship

Proyecto frontend desarrollado bajo la arquitectura modular y la metodología **BEM (Block, Element, Modifier)**, implementado como evidencia para el programa de formación del SENA (Ficha 3234206).

## Descripción de la Actividad Actual
En la sesión de hoy se llevaron a cabo las siguientes implementaciones técnicas y visuales:
* **Integración del Logotipo Corporativo:** Inserción del logotipo de "Dulcería Goldship" (`producto7.jpg`) en la cabecera principal (`.header-nav`), aplicando clases de estilo dedicadas (`.logo-img`) para un acoplamiento estético y un redimensionamiento óptimo.
* **Modularización del CSS:** Refactorización de la hoja de estilos en componentes atomizados bajo la estructura de carpetas `css/layout/` (`botones.css`, `catalogo.css`, `encabezado.css`, `menu-lateral.css`, `pie.css`, `tarjeta.css`), facilitando el mantenimiento y la escalabilidad del proyecto.
* **Ampliación del Catálogo:** Consolidación de la estructura HTML con la exhibición completa de los productos del catálogo web, asegurando la correcta semántica de etiquetas (`header`, `nav`, `aside`, `main`, `article`).

## Estructura del Repositorio
```text
css-3381732/
├── css/
│   └── layout/
│       ├── botones.css
│       ├── catalogo.css
│       ├── encabezado.css
│       ├── menu-lateral.css
│       ├── pie.css
│       └── tarjeta.css
├── imagenes/
│   └── producto1.jpg al producto7.jpg
├── index.html
├── style.css
└── README.md
Hallazgos: Arquitectura Total con Flexbox

1. Control del pie de página (min-height: 100vh y flex-direction: column)

Aplicar min-height: 100vh al contenedor global fue crucial porque asegura que la página cubra siempre toda la altura de la pantalla, sin importar si hay poco o mucho contenido. Al combinarlo con flex-direction: column, organizamos todos los bloques principales de arriba hacia abajo en una columna estricta, lo que nos permitió fijar el pie de página perfectamente en la parte inferior de la pantalla sin que suba de manera extraña cuando el contenido es corto.

2. Uso de la propiedad gap frente a márgenes laterales

La propiedad gap reemplazó por completo el uso excesivo y manual de márgenes (margin-right o margin-left) en los elementos de navegación. En lugar de calcular distancias para cada enlace o tener que eliminar el margen del último elemento, gap distribuye de forma automática y equitativa el espacio entre los hijos de manera limpia y uniforme.

3. Resiliencia de la tarjeta de producto (BEM, Custom Properties y Flexbox)

La combinación de BEM, las variables CSS (Custom Properties) y Flexbox permitió diseñar tarjetas de producto muy flexibles y resistentes. Gracias a esta unión, la tarjeta se adapta sin romperse a diferentes longitudes de texto en los títulos o descripciones, manteniendo siempre alineados elementos clave como la imagen, el cuerpo y el botón de compra de forma simétrica.