# 🏄‍♀️💙 Ventura Surf Co. – Premium Landing Page

[![Website Status](https://img.shields.io/badge/Status-Live-success.svg)](https://lna005.github.io/ventura-surf-co/)
[![Tech](https://img.shields.io/badge/Stack-HTML5%20|%20CSS3%20|%20JS-blue.svg)](#)
[![Accessibility](https://img.shields.io/badge/Accessibility-A11y-orange.svg)](#)
[![Made with love](https://img.shields.io/badge/Made%20with-💙-pink.svg)](#)

**Ventura Surf Co.** es una landing page de alto rendimiento diseñada para una escuela de deportes acuáticos en Fuerteventura 🌊. El proyecto combina una estética editorial moderna con optimizaciones técnicas de nivel profesional — y mucho amor por el océano. 🐚✨

🌐 **Demo en vivo →** [lna005.github.io/ventura-surf-co](https://lna005.github.io/ventura-surf-co/)

---

## ✨ Características Principales

### 💎 Diseño y Experiencia de Usuario (UX)
- 🖱️ **Cursor Personalizado Suave** — Implementado con `requestAnimationFrame` para una navegación fluida y orgánica.
- 🎨 **Diseño Editorial** — Tipografías contrastadas (`Bebas Neue`, `Syne`, `Crimson Pro`) y paleta inspirada en el entorno volcánico de Canarias.
- 📱 **Totalmente Responsivo** — Adaptado meticulosamente para móvil, tablet y escritorio.
- 💨 **Interacciones Dinámicas** — Gráficos de viento animados y tickers de texto infinito.

### 🛠️ Especificaciones Técnicas (Performance & SEO)
- ⚡ **Optimización de Animaciones** — Interpolación Lineal (Lerp) en el bucle de animación para reducir el uso de CPU.
- 🔍 **SEO & Open Graph** — Meta Tags completos para indexación óptima y previsualizaciones en redes sociales.
- 📊 **Datos Estructurados (JSON-LD)** — Esquema `Course` e `ItemList` para Rich Snippets en Google.
- ♿ **Accesibilidad (A11y)** — Clases `.sr-only`, etiquetas semánticas y atributos `aria` vinculados correctamente.

### 📩 Funcionalidad de Negocio
- 💌 **Formulario de Reserva Real** — Integración con **Formspree** para captura de leads directo al email, con validaciones nativas de HTML5.

---

## 🛠️ Tecnologías Utilizadas

| Tecnología | Uso |
|-----------|-----|
| HTML5 | Semántica avanzada |
| CSS3 | Custom Properties, Flexbox, Grid, Animaciones |
| JavaScript ES6+ | Intersection Observer API, rAF Animation Loop |
| JSON-LD | SEO Semántico |
| Formspree | Backend del formulario de reserva |

---

## 📦 Instalación y Uso

1. Clona el repositorio:
   ```bash
   git clone https://github.com/LNa005/ventura-surf-co.git
   ```

2. Abre `index.html` en tu navegador (o usa Live Server en VS Code 🤍).

3. Para que el formulario funcione, cambia el ID en el `action` del `<form>` por tu propio ID de Formspree:
   ```html
   <form action="https://formspree.io/f/TU_ID_AQUI" method="POST">
   ```

---

## 📋 Pendientes / TODO List 🩵

> Todo lo que queda por pulir para que esto esté *chef's kiss* ✨

### 🔴 Urgente (antes de compartir como portfolio)

- [ ] 🔗 **Enlazar Instagram real** — El botón del footer lleva a `#`, cámbialo por tu perfil real
- [ ] 💬 **Enlazar WhatsApp real** — Sustituir `href="#"` por `https://wa.me/34XXXXXXXXX` con tu número
- [ ] 📄 **Crear página de Política de Privacidad** — El enlace del footer lleva a `#` y es **obligatorio por RGPD** si el formulario recoge datos personales. Puedes usar un generador como [privacypolicygenerator.info](https://www.privacypolicygenerator.info/)
- [ ] 🖼️ **Añadir screenshot al README** — Meter una captura real del proyecto aquí arriba para que quede bonito en GitHub

### 🟡 Mejoras de contenido

- [ ] 📸 **Sustituir imágenes de Unsplash** — Reemplazar por fotos reales de la escuela, instructores y la playa de Corralejo (¡marca personal!)
- [ ] ⭐ **Sección de testimonios / reseñas** — Añadir valoraciones reales de alumnos o conectar con Google Reviews / Tripadvisor
- [ ] 🎒 **Página de detalle de cada curso** — Cada tarjeta tiene una flecha `→` que no lleva a ningún sitio todavía
- [ ] 🌍 **Versión en inglés / alemán** — El target turístico habla otros idiomas (Tom el instructor lo hace 😄)

### 🟢 Pulido técnico

- [ ] 🏷️ **Añadir favicon** — El sitio no tiene icono en la pestaña del navegador, añade uno acorde a la marca
- [ ] 📊 **Google Analytics o similar** — Para saber cuánta gente visita, desde dónde y qué secciones visitan más
- [ ] 🖼️ **Optimizar imágenes** — Convertir las imágenes a formato `.webp` para mejorar la velocidad de carga
- [ ] 🔒 **Honeypot en el formulario** — Campo oculto anti-spam para evitar bots en las reservas
- [ ] 🧪 **Testear el formulario de Formspree** — Hacer una reserva de prueba real y verificar que llega el email correctamente
- [ ] 📱 **Revisar en iOS Safari** — Algunos efectos CSS se comportan diferente en iPhone, vale la pena comprobarlo

### 💅 Nice to have (futuro)

- [ ] 🗓️ **Calendario de disponibilidad** — Integrar Calendly o similar para que los usuarios vean fechas disponibles
- [ ] 🌤️ **Widget de viento en tiempo real** — API de Windguru o Windy para mostrar las condiciones actuales de la playa
- [ ] 🖼️ **Galería de fotos** — Un lightbox con imágenes reales de las clases
- [ ] 💳 **Pago online** — Integrar Stripe para que las reservas se puedan confirmar con pago directo
- [ ] 📧 **Email de confirmación automático** — Con Formspree Pro o una función serverless (Netlify Functions)

---

## 👩‍💻 Autora

**Elena** 💙  
Hecho con ❤️ en Canarias 🌋🌊