# Catálogo Web de Dulcería Artesanal

Proyecto frontend desarrollado bajo la arquitectura modular y la metodología **BEM (Block, Element, Modifier)**, implementado como evidencia para el programa de formación del SENA (Ficha 3234206).

## Estructura del Proyecto
El proyecto organiza sus archivos y estilos de forma modular:

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
├── index.html
├── style.css
└── README.md
Hallazgos: Arquitectura BEM y Modularidad
1. Qué significa la sigla BEM y cómo se escribe visualmente
La sigla BEM responde al acrónimo en inglés de Block, Element, Modifier (Bloque, Elemento y Modificador). Representa una convención de nomenclatura orientada a otorgar transparencia y predictibilidad al diseño de interfaces. Visualmente se estructura mediante un bloque raíz independiente, un doble guion bajo para denotar un elemento dependiente (bloque__elemento) y un doble guion medio para designar una variante o estado (bloque--modificador).

2. Por qué dividir el CSS en varios archivos facilita el trabajo colaborativo
La fragmentación de la hoja de estilos en componentes atomizados dentro de la estructura modular previene los conflictos de convergencia en los sistemas de control de versiones. Al delegar responsabilidades específicas a ficheros especializados, múltiples desarrolladores pueden operar simultáneamente sobre distintos componentes visuales sin incurrir en modificaciones concurrentes sobre un único archivo central, reduciendo drásticamente las colisiones de código.

3. Cómo esta metodología evita la guerra de especificidad (Cascada) al mantener un peso plano
BEM neutraliza los conflictos derivados de la cascada descontrolada mediante la adopción de una estrategia de selectores planos de clase única. Al evitar la anidación excesiva o la dependencia de selectores de etiqueta complejos, se estandariza una especificidad constante (0,1,0), garantizando que cualquier regla pueda extenderse o sobrescribirse de forma predecible sin comprometer la integridad visual del sistema.