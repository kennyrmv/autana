# Design System — Autana

## Product Context
- **What this is:** Agencia de conversión digital para negocios de servicios en España. Web que convierte + bot de WhatsApp con IA real + automatizaciones.
- **Who it's for:** Dueños de negocios de servicios (clínicas estéticas, academias, asesorías, salones) en España. No técnicos, miden en reservas y clientes.
- **Space/industry:** Digital agency / automation / SMB services — Spain
- **Project type:** Marketing site (landing de agencia) + sistema de marca

## Brand Origin
Autana es el nombre del tepuy más misterioso de la Amazonía venezolana — una columna de roca de 1.300 metros que emerge sola de la selva. En lengua pemón (Venezuela), connota "árbol de la vida". Guiño personal del fundador a sus raíces venezolanas. El tepuy Autana emerge solo, imponente, sin necesitar nada alrededor. Eso es lo que hace Autana por los negocios de sus clientes.

## Nombre y Dominio
- **Nombre:** Autana
- **Dominio objetivo:** autana.es (verificar disponibilidad en nic.es antes de registrar)
- **Pronunciación:** au-TA-na
- **Tagline:** Tu negocio reserva solo mientras duermes.

## Aesthetic Direction
- **Direction:** Clean Professional con punch editorial
- **Decoration level:** Intentional (tipografía hace el trabajo principal; algún detalle de textura o fondo sutil)
- **Mood:** El único del sector que parece una herramienta seria (Stripe / Intercom) en lugar de una agencia dramática oscura. Transmite confianza al dueño de negocio no técnico.
- **Competitive gap:** Todos los competidores españoles serios (Flat101, Product Hackers) usan fondos oscuros y estética dramática. Autana ocupa el territorio libre: limpio, profesional, orientado a outcomes.
- **Reference sites:** glideapps.com (confianza sin dramatismo), stripe.com (herramienta que da confianza)

## Typography
- **Display/Hero:** Plus Jakarta Sans 800, letter-spacing -0.05em, line-height 1.0. Patrón de los top (Figma/Linear/Raycast): sans-serif pesado con tracking muy apretado. No serif — se probó Fraunces y se descartó (leía como editorial/revista, no como herramienta seria).
- **Body:** Plus Jakarta Sans 400–500. Párrafos, descripciones.
- **UI/Labels:** Plus Jakarta Sans 600–700 — botones, etiquetas de sección (uppercase + letter-spacing), nav links.
- **Data/Tables:** Plus Jakarta Sans 700 con tabular-nums — precios, métricas, ROI reports.
- **Code:** No aplica en el contexto de la agencia.
- **Loading:** Google Fonts CDN
  ```html
  <link href="https://fonts.googleapis.com/css2?family=Plus+Jakarta+Sans:wght@400;500;600;700;800&display=swap" rel="stylesheet">
  ```
- **Scale:**
  - xs: 0.6875rem (11px) — micro labels
  - sm: 0.75rem (12px) — badges, capslock labels
  - base: 0.875rem (14px) — UI secundario
  - md: 1rem (16px) — body estándar
  - lg: 1.0625rem (17px) — body destacado
  - xl: 1.125rem (18px) — card titles, subtítulos
  - 2xl: 1.375rem (22px) — section subtitles
  - 3xl: 1.75rem (28px) — section titles small
  - 4xl: 2.75rem (44px) — section titles
  - hero: clamp(2.5rem, 4vw, 3.75rem) — hero H1

## Color
- **Approach:** Restrained — un acento fuerte sobre base neutra cálida. El color es escaso y significativo.
- **Primary — Verde bosque:** #1B5E42 — acento principal. Crecimiento, salud, confianza. Nadie en el sector de agencias de automatización en Spain lo usa. Connota los tepuyes y la selva venezolana (coherencia con el nombre).
- **Primary dark:** #0D3320 — hover states, texto sobre verde
- **Primary tint:** #E8F5EE — fondos de badges, secciones destacadas, chat bubbles del bot
- **Primary mid:** #2D7A56 — variante intermedia
- **Background:** #F9F8F5 — casi blanco con calidez leve. Distinto del surface para que los cards destaquen.
- **Surface:** #FFFFFF — cards, chat card, modales, nav
- **Surface tint:** #F0F7F3 — fondo de elementos recibidos en chat, highlights
- **Text primary:** #0F1A14 — negro cálido con tinte verde, no negro puro
- **Text muted:** #6B7280 — descripciones, subtítulos secundarios
- **Text subtle:** #9CA3AF — timestamps, hints, placeholders
- **Border:** #E5E7EB — separadores, card borders
- **Border strong:** #D1D5DB — inputs, elementos con más definición
- **Semantic — success:** #1B5E42 (reutiliza verde primario)
- **Semantic — warning:** #CA8A04 (amber 600)
- **Semantic — error:** #EF4444 (red 500)
- **Dark mode:** Fondo #0A1410 (verde muy oscuro), surface #111C17, acento se aclara a #3DA672

## Spacing
- **Base unit:** 8px
- **Density:** Comfortable — generoso. Anti-densidad. El espacio en blanco es parte del diseño.
- **Scale:**
  - 2xs: 2px
  - xs: 4px
  - sm: 8px
  - md: 16px
  - lg: 24px
  - xl: 32px
  - 2xl: 48px
  - 3xl: 64px
  - 4xl: 96px

## Layout
- **Approach:** Grid-disciplined con punch editorial en el hero
- **Grid:** 12 columnas. 1 col mobile, 2 col tablet, 12 col desktop.
- **Max content width:** 1200px
- **Padding horizontal:** 2rem (desktop), 1.5rem (mobile)
- **Border radius:**
  - sm: 6px — inputs, pequeños elementos
  - md: 10px — cards secundarias
  - lg: 16px — cards principales, modales
  - full: 9999px — botones, badges, pills

## Motion
- **Approach:** Minimal-functional. Nada de animaciones flashy. Solo lo que ayuda a entender la UI.
- **Easing:** enter(ease-out) exit(ease-in) move(ease-in-out)
- **Duration:**
  - micro: 50–100ms — hover states, focus rings
  - short: 150–200ms — botones, badges
  - medium: 250–350ms — cards, modales
  - long: 400–500ms — page transitions (si aplica)

## Anti-Patterns (nunca usar)
- Gradientes morado/violeta como acento principal
- Grid de 3 columnas con iconos en círculos de colores
- Todo centrado con espaciado uniforme
- Border-radius uniforme y excesivo en todos los elementos
- Botones degradado como CTA principal
- Hero con foto de stock genérica
- Copy estilo "Built for X / Designed for Y"
- Fondo completamente negro como estética principal (eso es para la competencia)

## Decisions Log
| Fecha | Decisión | Rationale |
|-------|----------|-----------|
| 2026-04-07 | Nombre: Autana | Tepuy venezolano (Amazonas). "Árbol de la vida" en pemón. Guiño personal del fundador. autana.es sin DNS activo = probablemente libre. |
| 2026-04-07 | Verde bosque #1B5E42 como acento | Nadie en el sector lo usa. Connota crecimiento + salud. Coherente con origen natural del nombre. |
| 2026-04-07 | Fraunces serif para display | Riesgo creativo deliberado — descartado el 2026-04-08. Leía como editorial/revista, no como herramienta seria. |
| 2026-04-08 | Plus Jakarta Sans 800 para hero H1 | Patrón de los top 10 (Figma, Linear, Raycast): sans-serif 700-800 con tracking -0.05em. Usuario aprobó. |
| 2026-04-08 | Fondo #F9F8F5 + surface #FFFFFF | Casi blanco cálido para el bg, blanco puro para cards — contraste limpio sin frialdad clínica. |
| 2026-04-08 | Grain texture sutil (SVG fractalNoise, opacity 0.028) | Separa "flat" de "premium". Mismo tratamiento que monos.pro y Arc. |
| 2026-04-07 | Plus Jakarta Sans para body | Legible, moderno, no sobreutilizado como Inter/Roboto. |
| 2026-04-07 | Sistema de diseño creado | /design-consultation. Research visual: Glide, Flat101, Product Hackers, Chatbot Chocolate. |
