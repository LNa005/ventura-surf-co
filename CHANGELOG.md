# Changelog

Todos los cambios relevantes de este proyecto están documentados aquí.

El formato sigue el estándar [Keep a Changelog](https://keepachangelog.com/es/1.0.0/).

---

## [Unreleased]

### Por hacer
- Comprimir imágenes de cards a <150kb para mejorar rendimiento móvil
- Revisar en iOS Safari
- Añadir LinkedIn real cuando esté creado el perfil
- CHANGELOG.md — este archivo 😄

---

## [1.5.0] - 2026-03-08

### Added
- Animaciones de entrada con scroll usando `IntersectionObserver` — cards de cursos, instructores, testimonios y stats de viento entran con fade al hacer scroll
- Retrasos escalonados (`reveal-delay-1/2/3/4`) para que los elementos de una misma fila entren uno detrás de otro
- Comentarios completos en el JS explicando el *por qué* de cada decisión, no solo el *qué*
- JSDoc en la función `animateCursor()`

### Changed
- Flechas `→` de las cards de cursos: de círculo con borde semitransparente a círculo blanco sólido con flecha negra
- Al hacer hover la flecha cambia a color arena y crece ligeramente

---

## [1.4.0] - 2026-03-08

### Added
- Imagen hero servida con `<picture>` y `srcset`: `hero-mobile.webp` para móvil (<768px) y `hero.webp` para escritorio
- `<link rel="preload">` diferenciado por breakpoint para pre-cargar la imagen correcta en cada dispositivo

### Changed
- Hero: `background-image` de CSS reemplazado por `<img>` real con `fetchpriority="high"` y `loading="eager"` — esto permite que Lighthouse detecte el LCP correctamente
- Gradiente oscuro del hero movido a `::before` y textura de ruido a `::after` para mantener el mismo aspecto visual
- Google Fonts: carga bloqueante reemplazada por técnica `media="print" onload="this.media='all'"` + `<link rel="preconnect">` — evita que las fuentes retrasen el renderizado
- `og:image` actualizado con la URL real de GitHub Pages

### Performance
- LCP móvil: de error `NO_LCP` → 7.3s → 3.9s
- Lighthouse Desktop: Rendimiento 96 · Accesibilidad 92 · Prácticas 100 · SEO 91
- Lighthouse Mobile: Rendimiento 79 · Accesibilidad 93 · Prácticas 100 · SEO 91

---

## [1.3.0] - 2026-03-08

### Added
- 5 páginas de detalle de cada curso: `kitesurf.html`, `surf.html`, `windsurf.html`, `sup.html`, `privada.html`
- Cada página incluye: hero con imagen del curso, descripción, programa día a día, grid de qué incluye y sidebar sticky con precio y botón de reserva
- Mismo cursor personalizado, nav y footer que el resto del sitio
- Flechas `→` de las cards del index enlazadas a sus páginas de detalle

---

## [1.2.0] - 2026-03-08

### Added
- Sección de testimonios con 3 reseñas de alumnos (Marcos R., Laura P., Felix K.)
- Una reseña en alemán para reflejar el target turístico real de Fuerteventura
- Campo honeypot `_gotcha` en el formulario de Formspree para bloquear bots de spam
- `hero-mobile.webp` añadido a la carpeta `img/`

### Changed
- Todas las imágenes convertidas a `.webp` con squoosh.app
- Imagen del hero: añadido gradiente oscuro a la izquierda para mejorar la legibilidad del texto
- Card destacada de kitesurf: fondo cambiado de azul (`--blue`) a negro (`--black`)
- Margen negativo superior de `.curso-img` eliminado
- `.curso-num` reubicado debajo de la imagen en cards pequeñas

---

## [1.1.0] - 2026-03-07

### Added
- `privacy.html` — política de privacidad completa con 8 secciones RGPD
- `favicon.svg` — V de marca en rust con ola decorativa en sky
- Menú hamburguesa móvil: overlay a pantalla completa, cierre al hacer clic en cualquier link, bloqueo de scroll del body, `aria-expanded`
- `.gitignore` para archivos de sistema (Windows, Mac, VS Code)
- Screenshot del proyecto en `assets/preview.png` y añadido al README

### Changed
- Footer: enlaces de Instagram/WhatsApp reemplazados por GitHub (`https://github.com/LNa005`) y LinkedIn (pendiente de URL real)
- Menú móvil incluye también los enlaces de GitHub y LinkedIn

### Fixed
- Enlace de política de privacidad en footer: `href="#"` → `href="privacy.html"`

---

## [1.0.0] - 2026-03-06

### Added
- Landing page inicial con diseño editorial oscuro
- Tipografías: `Bebas Neue`, `Syne`, `Crimson Pro`
- Paleta de color: negro volcánico, blanco arena, rust, sky, sand
- Cursor personalizado con interpolación lineal (lerp) vía `requestAnimationFrame`
- Sección hero con texto animado al cargar
- Ticker de texto infinito animado con CSS
- Sección de cursos con grid featured + 4 cards pequeñas
- Sección de viento con gráfico de barras animado via `IntersectionObserver`
- Sección de instructores (Carlos, Sara, Tom)
- Sección de reserva con formulario integrado con Formspree (`xjgakbab`)
- Validaciones nativas HTML5 en el formulario
- Datos estructurados JSON-LD con esquema `Course` e `ItemList`
- Meta tags Open Graph para previsualizaciones en redes sociales
- Clases `.sr-only` y atributos `aria` para accesibilidad
- Diseño responsive para móvil, tablet y escritorio
- Publicación en GitHub Pages