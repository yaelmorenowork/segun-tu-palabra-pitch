# Según tu Palabra — pitch deck

Mazo interactivo de 14 slides en una sola página HTML autocontenida
(`index.html`). Ábrelo directamente en el navegador, o sirve la carpeta
(`npx http-server .`).

## Navegación

- Clic en la mitad derecha/izquierda de la pantalla, botones ‹ ›, o
  `→` / `espacio` / `←`.
- Cada slide avanza en 1–5 "beats" (entrada → desarrollo → cierre) antes de
  pasar a la siguiente, para poder marcar el ritmo durante el pitch en vivo.
- Barra superior segmentada: un segmento por slide (14 en total), el actual
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
final (slide 14, copia exacta de la portada).

## Estructura — 14 slides

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
7. **04 — El camino (1/2)** — "el recorrido de lectura" deja de ser una
   fila estática con flechas y pasa a ser una animación tipo
   scrollytelling: cada palabra (Leer, Entender, Reflexionar, Preguntar)
   ocupa el centro de la pantalla, protagonista, y se encoge hacia un
   rastro en la parte superior en cuanto entra la siguiente.
8. **04 — El camino (2/2) + comparación** — continúa exactamente el mismo
   mecanismo con las tres palabras restantes (Escribir, Compartir,
   Vivir); en el último beat el camino queda completo (las 7 palabras en
   el rastro superior) y aparece, debajo, con menor protagonismo pero
   tipografía notablemente mayor que en la versión anterior, la
   comparación de tres: Hallow (oración), Magisterium (conocimiento/IA),
   Según tu Palabra (Biblia + comunidad + herramientas + distribución).
9. **05 — Cómo llegamos** — reescrita como una secuencia numerada de 5
   pasos concretos (a quién nos dirigimos, cómo llegamos a ellos, qué les
   ofrecemos, cómo lo usan sus miembros, el objetivo de esta fase),
   reutilizando el mismo lenguaje visual de línea de tiempo del resto del
   mazo — línea vertical + punto — con número y desarrollo por paso.
10. **06 — El modelo** — las tres piezas que se complementan (App, Biblia
    física, Plataforma/comunidad) y, justo debajo de cada una, con el
    mismo peso visual que su descripción, quién paga por ella y cómo.
11. **07 — La inversión** — 100.000€ + un desglose proporcional real (los
    porcentajes por categoría fueron dados explícitamente) en un donut,
    reutilizando el mismo lenguaje visual del anillo de "El problema".
    Cada porción lleva su etiqueta y su porcentaje visibles en una
    leyenda, no sólo el color.
12. **08 — El recorrido** — línea de tiempo vertical protagonista (mismo
    componente que usaba antes también la slide "El plano"), 4 hitos
    personales.
13. **Cierre contemplativo** — sin badge, sin footer, centrado, mucho
    espacio en blanco. Dos citas, nada más.
14. **Portada (cierre)** — copia exacta de la slide 1: mismo marcado,
    mismo código, mismo bucle de palabras.

## Assets reutilizados sin tocar

Por petición explícita, estos elementos son exactamente los mismos que en
la versión anterior del mazo — sólo cambian de posición en el nuevo
orden, nunca su asset, su animación o su código:

- El mockup fotográfico de la Biblia (foto real, flotando, sombra
  despegada, márgenes con glow).
- El mockup del móvil con el vídeo real de la app en bucle.
- La slide de testimonios + código QR (el propio PNG del QR se actualizó
  al que subiste directamente).

## El desglose de "La inversión"

Esta es la única cifra del mazo con proporciones reales dadas por
categoría, así que el donut refleja el reparto exacto: Desarrollo 54%,
Sueldo fundadora (9 meses) 16%, Contingencia 14%, Primera tirada de
Biblias 4,5%, Constitución + legal 3,5%, Marketing/ventas institucional
3%, Gestoría 2%, Viajes institucionales 2%, Tecnología/hosting 1,2%. Los
colores son pasos de opacidad de la propia paleta navy más `--steel` /
`--steel-dark` / `--sky` — no se añadió ningún color nuevo.

## Pendiente / decisiones a validar

- **Slide "El camino" — badge "04 — Propuesta de valor"**: se repite en
  las dos slides del camino (1/2 y 2/2), igual que "03 — La solución" ya
  se repetía entre el móvil y la Biblia física en el mazo anterior —
  cámbialo si prefieres etiquetas distintas para cada mitad.
- **Slide "El modelo" — qué monetiza cada pieza**: el mensaje no
  especificaba qué categoría de monetización corresponde a cada una de
  las tres piezas, así que hice la asociación más directa: App →
  Funciones premium con IA; Biblia física → Contrato diócesis/colegio;
  Plataforma/comunidad → Suscripción parroquia + Transacciones (cursos,
  retiros, donaciones). Dime si prefieres otra distribución.
- **Slide "El recorrido"**: el badge "08 — El recorrido" es una etiqueta
  propia (el mensaje original no especificaba el texto exacto del badge
  para esta slide) — cámbialo si prefieres otro.
