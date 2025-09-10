# Curso de HTML W3Schools
Repositorio donde voy a ir poniendo todo el código que voy generando del curso de html de W3Schools
## Checklist de Optimización Web con HTML

Este documento recopila las mejores prácticas actuales para optimizar páginas web **solo usando HTML**, enfocándose en rendimiento, accesibilidad y experiencia de usuario.

---

### 1. Imágenes
- [ ] Usar formatos modernos: **WebP, AVIF** en lugar de JPG/PNG.
- [ ] `<img loading="lazy">` para carga diferida.
- [ ] Definir siempre `width` y `height` → evita CLS (Cumulative Layout Shift).
- [ ] `<picture>` con `srcset` y `sizes` → imágenes responsivas.
- [ ] `decoding="async"` para que la imagen no bloquee el renderizado.
- [ ] Atributo `alt` descriptivo → accesibilidad y SEO.

---

### 2. Videos y Multimedia
- [ ] `<video preload="metadata|none">` según necesidad.
- [ ] Usar `poster` para evitar cuadros en negro al cargar.
- [ ] `<iframe loading="lazy">` para embeds pesados (YouTube, mapas).

---

### 3. Recursos y Fuentes
- [ ] `<link rel="preload" as="font|style|script">` para recursos críticos.
- [ ] `<link rel="prefetch">` para recursos futuros.
- [ ] `<link rel="preconnect" href="...">` para dominios externos (CDN, fonts).
- [ ] Usar fuentes modernas: **WOFF2 > WOFF > TTF/OTF**.

---

### 4. SEO & Accesibilidad
- [ ] Uso correcto de etiquetas semánticas: `<header>`, `<main>`, `<article>`, `<section>`, `<footer>`.
- [ ] `<meta name="viewport" content="width=device-width, initial-scale=1.0">` para mobile.
- [ ] Todos los elementos interactivos accesibles: `aria-label`, `alt`, etc.

---

### 5. CSS y JS desde HTML
- [ ] `<link rel="stylesheet" media="print" onload="this.media='all'">` → carga diferida de CSS no crítico.
- [ ] `<script defer>` para scripts que dependen del DOM.
- [ ] `<script async>` para scripts que no dependen del DOM.

---

### 6. HTML Moderno para Layout y UI
- [ ] `<dialog>` para modales nativos sin JS.
- [ ] `<details>` + `<summary>` para acordeones nativos.
- [ ] `<template>` para cargar contenido sin renderizarlo hasta que sea necesario.
- [ ] `<picture>` + `srcset` + `sizes` → imágenes adaptables a pantalla y resolución.

---

### 7. Otros Consejos Generales
- [ ] Evitar inline styles grandes y código repetido.
- [ ] Evitar `<br>` excesivos, usar CSS para espaciado.
- [ ] Minificar HTML antes de publicar → menos KB transferidos.

