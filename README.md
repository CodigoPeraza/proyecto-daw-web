<div align="center">

# IDS-SOLUTION — Landing page responsive

**Página de aterrizaje adaptable a móvil construida con HTML y CSS puro, sin frameworks ni JavaScript.**

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![Responsive](https://img.shields.io/badge/Responsive-Design-4CAF50?style=for-the-badge&logo=googlechrome&logoColor=white)

</div>

![Banner del proyecto](images/banner.jpg)

## Descripción

Landing page desarrollada para la materia de Diseño de Aplicaciones Web. El proyecto sirve como ejercicio de maquetación responsive: incluye un encabezado con navegación, un menú hamburguesa implementado solo con CSS y una sección principal con imagen de fondo y llamada a la acción.

El enfoque está en demostrar dominio de layout, Flexbox, posicionamiento y adaptación a distintos tamaños de pantalla sin depender de librerías externas.

## Funcionalidades

- Encabezado con logotipo, navegación y llamada a la acción.
- Menú hamburguesa que se abre y cierra sin JavaScript, usando el estado `:checked` de un checkbox.
- Menú lateral a pantalla completa en dispositivos móviles.
- Sección principal con imagen de fondo, capa de superposición y texto destacado.
- Adaptación responsive mediante media query a partir de `764px`.
- Transiciones suaves en enlaces y en la apertura del menú.

## Stack técnico

- **HTML5** para la estructura.
- **CSS3** para el layout y la interacción.
- **Flexbox** para la distribución del header y el contenido.
- **Media queries** para el comportamiento responsive.
- **Tipografías del sistema** mediante la pila definida en CSS.

## Estructura

```text
proyecto-daw-web/
├── index.html      # Estructura de la landing
├── style.css       # Estilos, layout y responsive
├── images/
│   └── banner.jpg  # Imagen de fondo principal
└── README.md
```

## Cómo visualizarlo

No requiere instalación ni build. Basta con abrir `index.html` en el navegador.

Para servirlo con un servidor local:

```bash
python3 -m http.server 8000
```

Y visitar `http://localhost:8000`.

## Decisiones técnicas destacadas

- **Menú hamburguesa sin JavaScript:** un `input[type="checkbox"]` oculto controla la apertura del menú mediante el selector `#check:checked ~ .menu`. Es una técnica útil para prototipos rápidos y demuestra comprensión de selectores y estados CSS.
- **Layout con Flexbox:** el header usa `display: flex` con `justify-content: space-between` para separar logo y navegación.
- **Superposición con pseudo-elemento:** `#banner::before` crea una capa semitransparente sobre la imagen para mejorar el contraste del texto.
- **Responsive por media query:** en pantallas menores a `764px` el menú cambia a un panel fijo, los enlaces se apilan y se muestra el control de apertura/cierre.
- **Cero dependencias:** el proyecto se mantiene ligero y fácil de desplegar en cualquier hosting estático.

## Mejoras futuras

- Reemplazar los enlaces de ejemplo (`#`) por secciones reales.
- Añadir navegación accesible con `aria-*` y control de foco.
- Incorporar secciones de servicios, portafolio, contacto y footer.
- Añadir JavaScript solo si se requiere comportamiento adicional.
- Publicar una demo con GitHub Pages.

## Estado del proyecto

Maqueta funcional y responsive, pensada como base visual y ejercicio académico.

## Autor

**Francisco Javier Peraza** · [GitHub](https://github.com/CodigoPeraza) · [contacto.peraza@gmail.com](mailto:contacto.peraza@gmail.com)
