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

## Pendiente — necesito estos dos assets para terminarlas

- **Slide 4 — La Biblia de notas**: falta la foto o mockup real de la
  Biblia con el margen de anotación visible. El texto y el layout ya están
  construidos; la zona donde iría la imagen está marcada con un recuadro
  punteado que lo indica explícitamente (no hay ningún placeholder
  genérico haciendo pasar por definitivo).
- **Slide 10 — Lo que pido**: falta el desglose real del panel financiero
  interactivo (Chart.js) — evolución de ingresos, burn rate o runway a 36
  meses. Mismo tratamiento: recuadro punteado marcando lo que falta, cifra
  y texto ya construidos.

Cuando me pases esos dos assets, sustituyo los recuadros por el contenido
real sin tocar el resto del sistema.

### Notas menores, no bloqueantes

- Slide 7: el desglose exacto de "retiros" frente a los demás canales
  institucionales no estaba disponible en esta sesión — los canales se
  listan sin desglosar, tal y como se indicó como opción válida.
- El mapa de la slide 7 es una ilustración vectorial abstracta (cluster de
  puntos), no un mapa geográfico real — generada porque no había un asset
  de mapa disponible.
