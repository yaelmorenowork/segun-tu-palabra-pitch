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

- **Slide 4 — La Biblia de notas**: una única foto real (la del margen
  ancho con anotaciones a mano) con fondo genuinamente transparente —
  ya no queda ningún rastro de la foto anterior. Flota directamente
  sobre el degradado de la slide, sin tarjeta ni caja detrás, con una
  sombra suave y despegada debajo y un balanceo vertical mínimo y
  continuo. La secuencia se mantiene: llega y se sostiene un instante,
  luego los márgenes se convierten en protagonistas (su propio glow) y
  las palabras clave entran una a una.
- **Slide 9 — Dos escenarios**: bajo cada título (Conservador/Base), su
  propia gráfica de barras agrupadas Ingresos vs. Gastos por año (Año
  1/2/3) — datos reales del motor del panel, mismos colores del sistema
  (navy sólido para Ingresos, acero/lavanda para Gastos, nunca semáforo
  rojo/verde), un único eje compartido entre ambas gráficas para que la
  comparación entre escenarios sea honesta. Las barras crecen desde 0 al
  cargar la slide, con tooltip al pasar el cursor sobre cada una.
- **Slide 10 — Lo que pido**: dos zonas claramente distintas — arriba/
  izquierda, la cifra de la inversión (200.000€) y qué cubre; abajo/
  derecha, una tarjeta aparte con el desglose real del gasto a 3 años
  (~419.000€): Producto, Equipo, Marketing, Contenido, Operaciones, cada
  una con su cifra y porcentaje. El contador se completa primero;
  después entra la tarjeta del desglose como una unidad, con su etiqueta
  apareciendo primero y las barras desplegándose de izquierda a derecha.
- **Slide 8 — Un modelo simple**: sin la línea divisoria entre los
  bloques Biblia/App; cada bloque incluye ahora su desglose (precio,
  traducción y canales de la Biblia; modelo freemium y suscripciones de
  la app).
- **Slide 5 — Cinco modos de estudio**: layout a dos columnas. A la
  derecha, un mockup de móvil grande (marco oscuro, esquinas
  redondeadas, dynamic island) con el vídeo real de la app en bucle
  (silenciado, autoplay, llena la pantalla del mockup sin bandas
  negras). El vídeo original (12MB) se recomprimió a H.264/CRF 20 sin
  tocar su contenido (mismos 580×1300, ~56s, sin audio) para mantener el
  peso de la página razonable — visualmente no se distingue del
  original. A la izquierda, las 5 tarjetas de "modos" en pila con
  solapamiento parcial (mismo efecto de tarjeta blanca/rotación/sombra
  de antes) y el bloque de texto alineado a la izquierda debajo.

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
