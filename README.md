# Catálogo Formativo — Cátedra Paradigmas 3

Trabajo áulico individual de la cátedra **Paradigmas y Lenguajes de Programación 3** (UTN).
Interfaz web construida con **HTML5 y CSS3 puros**, sin frameworks ni JavaScript,
servida localmente con **XAMPP** (Apache) y versionada con **Git**.

## Páginas

| Archivo              | Contenido                                              |
|----------------------|--------------------------------------------------------|
| `index.html`         | Portada principal del catálogo                         |
| `listado_tabla.html` | Listado de productos usando `<table>`                  |
| `listado_box.html`   | Listado de productos en tarjetas con CSS Grid          |
| `detalle_placa.html`       | Ficha técnica de la placa de video               |
| `detalle_procesador.html` | Ficha técnica del procesador                      |
| `detalle_memoria.html`    | Ficha técnica de la memoria RAM                   |
| `comprar.html`       | Formulario de compra (datos del cliente + productos)   |

## Estructura

```
catalogo-paradigmas3/
├── index.html
├── listado_tabla.html
├── listado_box.html
├── detalle_placa.html
├── detalle_procesador.html
├── detalle_memoria.html
├── comprar.html
├── css/
│   └── estilos.css
└── img/
    ├── index.jpeg
    ├── ram32.jpeg
    ├── rx7800xt.jpeg
    └── ryzen77800x3d.jpeg
```

## Cómo ejecutarlo

1. Copiar la carpeta dentro de `C:\xampp\htdocs\`.
2. Iniciar **Apache** desde el panel de control de XAMPP.
3. Abrir el navegador en `http://localhost/catalogo-paradigmas3/`.

## Decisiones técnicas

- **Una ficha por producto**: al ser un sitio estático, cada producto necesita su propio archivo HTML. Las tres fichas comparten la misma clase `.ficha`, así que el CSS no se duplica.
- **Una sola hoja de estilos** (`css/estilos.css`) compartida por las cinco páginas, para no repetir código.
- **Variables CSS** (`:root`) para centralizar la paleta de colores.
- **Flexbox** para la barra de navegación y **CSS Grid** para la grilla de tarjetas.
- **Diseño adaptable Desktop-First**: los `@media` usan `max-width`, partiendo del diseño de escritorio hacia pantallas menores.
