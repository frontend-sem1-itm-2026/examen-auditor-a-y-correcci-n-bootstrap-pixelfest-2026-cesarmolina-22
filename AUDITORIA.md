# Auditoría rápida — PixelFest 2026

| # | Problema detectado | Categoría | ¿Por qué es problema? |
|---|---|---|---|
| 1 |  |  |  |
| 2 |  |  |  |
| 3 |  |  |  |
| 4 |  |  |  |
| 5 |  |  |  |
| 6 |  |  |  |


## Problema 1 — Navbar no responsive
La barra de navegación no se adapta correctamente a pantallas pequeñas porque no utiliza el componente `navbar-expand` de Bootstrap ni el botón hamburguesa.

Solución:
Se agregó `navbar-expand-lg` y `navbar-toggler` para permitir navegación responsive.

---

## Problema 2 — Falta meta viewport
El documento no tiene la etiqueta meta viewport, lo que provoca que la página no sea realmente responsive en dispositivos móviles.

Solución:
Se agregó:

<meta name="viewport" content="width=device-width, initial-scale=1">

---

## Problema 3 — Uso incorrecto del Grid System
Algunos elementos no utilizan correctamente `container`, `row` y `col`, lo que provoca que el contenido se vea desordenado.

Solución:
Se reorganizó el layout utilizando correctamente:

container → row → col

---

## Problema 4 — Imágenes no responsivas
Las imágenes no tienen la clase `img-fluid`, lo que provoca que se desborden en pantallas pequeñas.

Solución:
Se agregó la clase:

class="img-fluid"

---

## Problema 5 — Mala jerarquía visual
Los títulos y textos no tienen una jerarquía clara, lo que dificulta entender las secciones.

Solución:
Se utilizaron encabezados adecuados (`h1`, `h2`, `h3`) y espaciado con Bootstrap (`mb-4`, `py-5`).

---

## Problema 6 — Links sin funcionalidad
Algunos botones y enlaces no redirigen a ninguna sección de la página.

Solución:
Se agregaron `id` a las secciones y enlaces funcionales con `href="#seccion"`.

---

## Problema 7 — Falta de espaciado
La página tiene elementos muy juntos sin márgenes ni padding.

Solución:
Se agregaron utilidades de Bootstrap como:

py-5  
mb-4  
g-4