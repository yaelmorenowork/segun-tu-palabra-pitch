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
2. **01 — El plano** — texto a la izquierda; línea de tiempo vertical
   decorativa a la derecha (redacción de los textos bíblicos → primera
   traducción → hoy).
3. **02 — El problema** — el 67% en un anillo circular (mismo lenguaje
   visual que la barra de progreso superior, en redondo).
4. **03 — La solución** — mockup del móvil con el vídeo real de la app en
   bucle; título + dos filas de chips (modos de estudio / público
   ampliado).
5. **03 — La solución** (biblia física) — mismo mockup fotográfico de la
   Biblia que la versión anterior del mazo, con un texto breve al lado.
6. **Primeras pruebas** — testimonios + QR, reutilizada tal cual (sin
   badge, para no repetir "03" una tercera vez seguida).
7. **04 — El mercado** — grid de tres cifras (Hallow en Latinoamérica,
   Colombia, México resaltado en el acento azul/lavanda).
8. **05 — Cómo llegamos** — tres tarjetas iguales con icono simple
   (diócesis, creadores de contenido, ocasiones de regalo).
9. **06 — El modelo** — flujo horizontal con flechas: suscripción → Biblia
   física → licencias B2B, con nota sobre el margen del canal tradicional.
10. **07 — La inversión** — 80.000€ + la barra segmentada del header
    reutilizada a mayor escala, mostrando las seis categorías del reparto.
    Las categorías se dieron sin proporciones individuales, así que los
    segmentos son deliberadamente iguales — una lista, nunca una cifra
    inventada.
11. **08 — El recorrido** — línea de tiempo vertical protagonista (mismo
    componente que la slide 2), 4 hitos personales.
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
  QR sigue sin fondo transparente real (confirmado en una pasada
  anterior) — mantiene su tarjeta con sombra suave.
- **Slide "El recorrido"**: el badge "08 — El recorrido" es una etiqueta
  propia (el mensaje original no especificaba el texto exacto del
  badge para esta slide) — cámbialo si prefieres otro.
- **Slide "La inversión"**: las seis categorías del reparto de 80.000€
  se muestran como segmentos iguales porque no se me dieron proporciones
  o cifras individuales por categoría — si tienes esos números, dímelos
  y ajusto los anchos de cada segmento a la proporción real.
