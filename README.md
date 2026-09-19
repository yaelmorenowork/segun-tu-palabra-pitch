# Según tu Palabra — pitch deck

Mazo interactivo de 13 slides en una sola página HTML autocontenida
(`index.html`). Ábrelo directamente en el navegador, o sirve la carpeta
(`npx http-server .`).

## Navegación

- Clic en la mitad derecha/izquierda de la pantalla, botones ‹ ›, o
  `→` / `espacio` / `←`.
- Cada slide avanza en 1–4 "beats" (entrada → desarrollo → cierre) antes de
  pasar a la siguiente, para poder marcar el ritmo durante el pitch en vivo.
- Barra superior segmentada: un segmento por slide (13 en total), el actual
  resaltado.
- Puntos inferiores: beats dentro de la slide actual (se reinician en cada
  slide nueva).

## Sistema visual

Heredado tal cual del sistema original aprobado — no redefinido en esta
pasada: paleta navy/acero/crema, glassmorphism en tarjetas, atmósfera de
degradado difuminado (nunca a pantalla completa), tipografía de sistema
estilo Apple, mecanismo de highlight sobre texto. Componentes recurrentes:
logo arriba-izquierda, categoría arriba-derecha, badge píldora "0N —
Nombre", footer abajo-izquierda, navegación tipo carrusel abajo-centro.

Cada slide tiene su propio grid (centrado puro, asimétrico, grid de
tarjetas, flujo horizontal, línea de tiempo vertical, dos columnas…) y su
propia transición de entrada/salida — no hay dos consecutivas con el mismo
movimiento, salvo el eco deliberado entre la portada (slide 1) y el cierre
final (slide 13, copia exacta de la portada).

## Estructura — 13 slides

1. **Portada** — sin badge. "La Palabra es " + efecto typewriter en bucle
   continuo (vida, camino, verdad, alimento, promesa, dirección, Cristo).
2. **01 — El plano** — texto a la izquierda; el lado derecho queda en
   blanco a propósito (vacío intencional, sin línea de tiempo ni ningún
   otro elemento de relleno).
3. **02 — El problema** — el 67% en un anillo circular (mismo lenguaje
   visual que la barra de progreso superior, en redondo); subtítulo a
   tamaño grande, a la par visual de la cifra.
4. **03 — La solución** — mockup del móvil con el vídeo real de la app en
   bucle; los modos de estudio son el elemento protagonista — cuatro en
   total (Histórico, Teológico, Etimológico, Pastoral) — con una
   animación tipo "ventana": cada uno aparece y se asienta antes de que
   aparezca el siguiente, dejando una pausa real entre cada uno para
   marcar el ritmo en un pitch en vivo.
5. **03 — La solución** (biblia física) — mismo mockup fotográfico de la
   Biblia que la versión anterior del mazo, con un texto breve al lado.
6. **Primeras pruebas** — testimonios + QR, reutilizada tal cual (sin
   badge, para no repetir "03" una tercera vez seguida).
7. **04 — Propuesta de valor** — flujo horizontal animado con flechas,
   en secuencia: Leer → Entender → Reflexionar → Preguntar → Escribir →
   Compartir → Vivir. Debajo, con menor protagonismo (tipografía más
   pequeña, menor contraste), una comparación de tres: Hallow (oración),
   Magisterium (conocimiento/IA), Según tu Palabra (Biblia + comunidad +
   herramientas + distribución).
8. **05 — Cómo llegamos** — tres tarjetas iguales con icono simple
   (diócesis/ministerio hispano, creadores de contenido, ocasiones de
   regalo).
9. **06 — El modelo** — tres piezas que se complementan (no un flujo
   secuencial): App (el corazón, el hábito diario), Biblia física (la
   puerta de entrada), Plataforma/comunidad (el canal y el motor
   económico); debajo, compacta, la monetización de cada capa
   (suscripción parroquia, contrato diócesis/colegio, transacciones,
   funciones premium con IA).
10. **07 — La inversión** — 100.000€ + la barra segmentada del header
    reutilizada a mayor escala, mostrando las ocho categorías del
    reparto. Las categorías se dieron sin proporciones individuales, así
    que los segmentos son deliberadamente iguales — una lista, nunca una
    cifra inventada.
11. **08 — El recorrido** — línea de tiempo vertical protagonista (mismo
    componente que se usaba antes en la slide 2, ahora sólo aquí), 4
    hitos personales.
12. **Cierre contemplativo** — sin badge, sin footer, centrado, mucho
    espacio en blanco. Dos citas, nada más.
13. **Portada (cierre)** — copia exacta de la slide 1: mismo marcado,
    mismo código, mismo bucle de palabras.

## Assets reutilizados sin tocar

Por petición explícita, estos tres elementos son exactamente los mismos
que en la versión anterior del mazo — sólo cambian de posición en el
nuevo orden, nunca su asset, su animación o su código:

- El mockup fotográfico de la Biblia (foto real, flotando, sombra
  despegada, márgenes con glow).
- El mockup del móvil con el vídeo real de la app en bucle.
- La slide de testimonios + código QR.

## Pendiente / decisiones a validar

- **Slide 6 — QR de prueba** (dentro de "Primeras pruebas"): el PNG del
  QR es el que subiste (`qr-code.png`) — verificado con inspección
  directa de píxeles (PIL/numpy): es modo RGB, **sin canal alfa real**,
  100% opaco. No es transparente, así que se mantiene con su tarjeta y
  sombra suave existentes en vez de fingir transparencia o añadirle un
  fondo propio. Si me pasas una versión con transparencia real, la
  cambio para que flote sin tarjeta.
- **Slide "El recorrido"**: el badge "08 — El recorrido" es una etiqueta
  propia (el mensaje original no especificaba el texto exacto del
  badge para esta slide) — cámbialo si prefieres otro.
- **Slide "Propuesta de valor"**: el badge "04 — Propuesta de valor" es
  una etiqueta propia (tampoco se especificó el texto exacto) — cámbialo
  si prefieres otro.
- **Slide "La inversión"**: las ocho categorías del reparto de 100.000€
  se muestran como segmentos iguales porque no se me dieron proporciones
  o cifras individuales por categoría — si tienes esos números, dímelos
  y ajusto los anchos de cada segmento a la proporción real.
