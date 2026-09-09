# Según tu Palabra — pitch deck

Mazo interactivo de 11 slides en una sola página HTML autocontenida
(`index.html`). Ábrelo directamente en el navegador, o sirve la carpeta
(`npx http-server .`).

## Navegación

- Clic en la mitad derecha/izquierda de la pantalla, botones ‹ ›, o
  `→` / `espacio` / `←`.
- Cada slide avanza en 1–3 "beats" (entrada → desarrollo → cierre) antes de
  pasar a la siguiente, para poder marcar el ritmo durante el pitch en vivo.
- Barra superior segmentada: un segmento por slide (11 en total), el actual
  resaltado — igual que el patrón de progreso de las pantallas de onboarding
  de la app.
- Puntos inferiores: beats dentro de la slide actual (se reinician en cada
  slide nueva).

## Sistema visual

Heredado tal cual del primer preview (slides 1–3) aprobado — no redefinido
en esta pasada: paleta navy/acero/crema, glassmorphism en tags y botones,
atmósfera de degradado difuminado (nunca a pantalla completa), tipografía de
sistema estilo Apple (`-apple-system` / Segoe UI / Inter como respaldo web),
mecanismo de highlight sobre texto. Componentes recurrentes en las 11 slides:
logo arriba-izquierda, etiqueta de sección arriba-derecha, badge píldora
"0N — Nombre", pie de página, navegación tipo carrusel.

Cada slide tiene su propio grid (centrado puro, asimétrico, tercios,
abanico de columnas, capas, split vertical, dos zonas lado a lado…) y su
propia transición de entrada/salida — no hay dos consecutivas con el mismo
movimiento, salvo los dos ecos deliberados: la apertura y el cierre
(mismo "dissolve" suave, espejo), y el 67 % / 200.000 € (mismo conteo
ascendente).

## Estado de los assets

- **Slide 4 — La Biblia de notas**: foto real (cerrada + abierta), con
  fondo genuinamente transparente. El libro flota directamente sobre el
  degradado de la slide — sin tarjeta ni caja detrás — con una sombra
  suave y despegada debajo y un balanceo vertical mínimo y continuo,
  tanto cerrado como abierto.
- **Slides 9 y 10 — Dos escenarios / Lo que pido**: gráficas reales,
  interactivas, construidas a partir de los 36 valores mensuales exactos
  del panel financiero (sin cifras aproximadas ni inventadas). Un punto
  recorre cada línea mes a mes en bucle continuo y lento, con la cifra
  real de ese mes junto al punto, marcas en los meses 12/24/36 y un
  tooltip al pasar el cursor. La slide 9 compara Conservador vs. Base
  (dos líneas); la slide 10 muestra solo el escenario Conservador (una
  línea con área rellena) — diseño visual distinto entre ambas, misma
  lógica de interacción.

### Pendiente

- **Slide 6 — QR de prueba**: el PNG del QR que se usa (`qr-code.png`)
  tiene canal alfa pero está totalmente opaco (fondo blanco sólido, no
  transparente). Por eso el QR sigue mostrando una tarjeta con sombra
  suave alrededor en vez de integrarse directamente sobre el fondo — no
  se ha añadido ningún fondo propio para compensarlo. El QR y el texto
  ya están notablemente más grandes, legibles desde el fondo de una
  sala. Si me pasas una versión con transparencia real, quito la tarjeta
  y lo dejo flotando igual que la Biblia.

### Notas menores, no bloqueantes

- Slide 7: el desglose exacto de "retiros" frente a los demás canales
  institucionales no estaba disponible en esta sesión — los canales se
  listan sin desglosar, tal y como se indicó como opción válida.
- El mapa de la slide 7 es una ilustración vectorial abstracta (cluster de
  puntos), no un mapa geográfico real — generada porque no había un asset
  de mapa disponible.
