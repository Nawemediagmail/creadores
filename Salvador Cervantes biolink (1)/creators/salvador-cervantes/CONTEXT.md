# Contexto: Biolink de Salvador Cervantes
> Actualizado: 18 Jun 2026 — para continuar trabajo en otro chat

---

## ¿Qué es este proyecto?
Página de biolink (tipo Linktree) para el creator **Salvador Cervantes** — Influencer y Content Creator.  
Hecho con el NAWEMEDIA Design System. Archivo principal: `creators/salvador-cervantes/biolink.dc.html`

---

## Estado actual del diseño

### Visual
- **Fondo**: Gradiente azul claro a blanco (`#DDEEFF → #FFFFFF`)
- **Figuras de fondo (fixed, decorativas)**:
  - **Izquierda**: `bg-photo.png` — pose con gorra roja, filtro azul monocromático, opacidad 22%
  - **Derecha**: `hero-right.png` — HERO PNG transparente cuerpo completo, mismo filtro azul, opacidad 22%
- **Cards de links**: `rgba(255,255,255,0.85)` + `backdrop-filter: blur(14px)` — efecto glassmorphism
- **Tipografía**: Bebas Neue (headers/nombre), Montserrat (body/subtítulos)
- **Paleta**: Azul navy `#0B1D4A`, azul medio `#1565C0`, azul claro `#42A5F5`, celeste `#7AABDA`
- **Animaciones**: `fadeUp` staggered en todos los elementos, `ringPulse` en el avatar

### Contenido
- **Nombre**: Salvador Cervantes
- **Tagline**: *"Parezco un Santo pero puedo ser tu Diablo"*
- **Tags**: Influencer · Content Creator
- **CTA principal**: "¡Subscríbete a mis canales!" (botón azul gradiente arriba de todo)

### Redes sociales (en orden)
| Red | Ícono | Handle actual | URL |
|---|---|---|---|
| Instagram | `icons/instagram.png` | @salvadorcervantes | ⚠️ FALTA URL REAL |
| TikTok | `icons/tiktok.png` | @salvadorcervantes | ⚠️ FALTA URL REAL |
| OnlyFans | `icons/onlyfans.png` | Contenido exclusivo | ⚠️ FALTA URL REAL |
| Twitter/X | `icons/x.png` | @salvadorcervantes | ⚠️ FALTA URL REAL |
| Telegram | `icons/telegram.png` | @salvadorcervantes | ⚠️ FALTA URL REAL |
| WhatsApp | `icons/whatsapp.png` | Escríbeme directo | ⚠️ FALTA URL REAL |

### Galería (debajo de los botones)
Grid 2 columnas, 5 fotos:
- `gallery/foto-3.jpg`, `gallery/foto-4.jpg`, `gallery/foto-5.jpg`, `gallery/foto-6.jpg`
- `gallery/foto-7.jpg` — ancho completo (span 2 cols), aspect ratio 3:2

---

## Estructura de archivos

```
creators/salvador-cervantes/
├── biolink.dc.html          ← ARCHIVO PRINCIPAL
├── support.js               ← runtime DC (no editar)
├── perfil.png               ← foto de perfil circular (avatar)
├── photo.jpg                ← foto cuerpo completo (no usada en diseño actual)
├── bg-photo.png             ← figura decorativa IZQUIERDA
├── bg-photo-right.png       ← (no usada — reemplazada por hero-right.png)
├── hero-right.png           ← figura decorativa DERECHA (HERO PNG transparente)
├── icons/
│   ├── instagram.png
│   ├── tiktok.png
│   ├── onlyfans.png
│   ├── x.png
│   ├── telegram.png
│   └── whatsapp.png
└── gallery/
    ├── foto-3.jpg
    ├── foto-4.jpg
    ├── foto-5.jpg
    ├── foto-6.jpg
    └── foto-7.jpg
```

---

## Pendientes / posibles próximos pasos

1. **Agregar URLs reales** a los 6 botones de redes (todos tienen `href="#"`)
2. **Handles reales**: confirmar si @salvadorcervantes es correcto en todas las redes
3. **Lightbox en galería**: hacer que las fotos abran en grande al hacer click
4. **Foto de perfil**: actualmente usa `perfil.png` (cuadrada) — ajustar `object-position` si el recorte no queda bien
5. **Optimización mobile**: revisar en iPhone real (diseño preview 390×844)
6. Posibles mejoras: añadir sección de eventos, embed de video, o botón de contacto/booking

---

## Design System
NAWEMEDIA Design System — ID: `64053915-7048-43a8-aaa0-e36e7d4e5419`
- Fuentes: Bebas Neue, Montserrat
- Este biolink usa paleta custom azul/blanco (no el modo oscuro neon del DS principal)
- Footer: "Powered by NAWEMEDIA"
