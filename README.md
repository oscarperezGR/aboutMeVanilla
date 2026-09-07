# LandingPageAboutMe

Página personal de presentación desarrollada con HTML5 y CSS3, sin librerías ni
frameworks. Proyecto individual del bootcamp de desarrollo web de JM Factoría.

## Enlaces

- **Página publicada:**  https://oscarperezgr.github.io/aboutMeVanilla/
- **Repositorio:** https://github.com/oscarperezGR/aboutMeVanilla.git

## Captura

![Vista general de la página](assets/screenshot.jpg)

## Descripción

Una landing page de una sola pantalla en la que me presento. Está dividida en
cinco secciones, cada una combinando texto e imagen:

- Nombre, apellidos y fotografía
- Lugar de nacimiento y nacionalidad
- Aficiones
- Estudios y centros donde los realicé
- Recorrido personal y profesional

La estructura sigue el esquema `header` / `main` / `footer`, con la navegación
principal enlazada a cada sección mediante anclas.

## Tecnologías

- HTML5 semántico
- CSS3: Flexbox, variables personalizadas, media queries
- Tipografías Newsreader e Inter servidas desde Google Fonts
- Imágenes generadas con inteligencia artificial generativa

No se ha utilizado ninguna librería ni framework de CSS.

## Estructura del proyecto

```text
LandingPageAboutMe/
├── index.html
├── styles.css
├── README.md
└── assets/
    ├── profilePhoto.jpg
    ├── birthplacePhoto.jpg
    ├── hobbiesPhoto.jpg
    ├── studiesPhoto.jpg
    ├── journeyPhoto.jpg
    └── screenshot.jpg
```

## Decisiones de desarrollo

- **Variables CSS.** Los colores, espaciados y tipografías se definen una sola
  vez en `:root`, de forma que cualquier cambio de estilo se hace desde un único
  punto del archivo.
- **Secciones alternas.** Las cinco secciones comparten la clase
  `profile-section`. Las que invierten el orden de texto e imagen añaden
  `profile-section--reverse`, que solo aplica `flex-direction: row-reverse`.
- **Diseño adaptable.** A partir de 860 píxeles de ancho hacia abajo, las
  secciones pasan de dos columnas a una sola.
- **Accesibilidad.** Cada sección está asociada a su título con
  `aria-labelledby`, todas las imágenes llevan texto alternativo descriptivo y
  los elementos interactivos muestran un foco visible al navegar con teclado.

## Cómo verlo en local

```bash
git clone https://github.com/oscarperezGR/aboutMeVanilla.git
cd AboutMeVanilla
```

Abre `index.html` en el navegador. No requiere instalación ni servidor.

## Autoría

Oscar Pérez — bootcamp de desarrollo web, 2026.
