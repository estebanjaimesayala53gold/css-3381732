# Momento 2: Misión de Apropiación - Catálogo Web de Dulcería

## Descripción Académica del Proyecto
La presente obra digital constituye el desarrollo de la interfaz web para una dulcería artesanal, estructurada bajo los principios de la semántica en HTML5 y las normas de diseño tradicional en CSS. Conforme a las directrices de la misión, el planteamiento arquitectónico prescinde por completo de maquetadores modernos (tales como Flexbox o Grid), cimentando su disposición visual en el modelo de caja clásico (márgenes, rellenos y restricciones de bloque).

---

## Estructura del Repositorio

```text
├── dulces/
│   └── dulces.jpg      # Recurso gráfico de la temática de dulcería
├── index.html          # Marcado semántico de la aplicación web
├── style.css           # Hoja de estilos y gestión de especificidad
└── README.md           # Memoria técnica del proyecto y cálculo de puntos
1. Análisis de Especificidad y Cascada CSS
Para la resolución de conflictos visuales sin incurrir en la mala práctica del uso de la directiva !important, se ha evaluado el peso matemático de los selectores según la jerarquía estándar:

Etiquetas (Elementos): 1 punto de valor base.

Clases (class): 10 puntos de valor intermedio.

Identificadores (id): 100 puntos de valor superior.

Refactorización del Sistema Plano
Con el propósito de estandarizar la especificidad y prevenir sobreescrituras imprevistas de la cascada, el código CSS ha sido refactorizado, erradicando los selectores basados en ID y consolidando un sistema plano fundamentado exclusivamente en etiquetas y clases (por ejemplo, .btn-comprar), garantizando así un mantenimiento óptimo y una jerarquía limpia.

2. Control de Versiones (Git y GitHub)
El flujo de trabajo ha sido confinado y respaldado localmente mediante ramas de desarrollo, asegurando la trazabilidad de los commits previos a la subida final a la nube:

Bash
# Secuencia de comandos ejecutada para la consolidación y envío del trabajo
git checkout -b develop
git add .
git commit -m "feat(styles): maquetar catalogo semantico y aplicar jerarquia CSS"
git push origin develop