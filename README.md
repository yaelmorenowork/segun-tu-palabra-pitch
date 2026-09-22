# Según tu Palabra — pitch deck

Mazo interactivo de 13 slides en una sola página HTML autocontenida
(`index.html`). Ábrelo directamente en el navegador, o sirve la carpeta
(`npx http-server .`).

## Navegación

- Clic en la mitad derecha/izquierda de la pantalla, botones ‹ ›, o
  `→` / `espacio` / `←`.
- Cada slide avanza en 1–5 "beats" (entrada → desarrollo → cierre) antes de
  pasar a la siguiente, para poder marcar el ritmo durante el pitch en vivo.
- Excepción: en "Propuesta de valor" el recorrido de palabras se reproduce
  solo, con temporización fija, en cuanto se entra en la slide — no hace
  falta clic para avanzar cada palabra (sólo el beat siguiente, con la
  comparación, sigue esperando un clic).
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
   continuo (vida, camino, verdad, alimento, promesa, dirección, Cristo),
   con el nombre del proyecto ("Según tu Palabra") debajo, en mayúsculas
   pequeñas.
2. **01 — El plano** — texto a la izquierda, cerrando con dos frases
   ("No es un problema de fe..." y "Nos quedamos a la puerta de un
   edificio enorme."); a la derecha, la idea protagonista de la slide —
   "Según tu Palabra quiere ser esa puerta." — con más peso tipográfico
   que cualquier otro texto en ella.
3. **02 — El problema** — grid de dos columnas: a la izquierda, el 67%
   en un anillo circular (mismo lenguaje visual que la barra de progreso
   superior) y el texto (con "(Pew Research)" forzado a no partirse); a
   la derecha, una lista de apps católicas — Hallow, iBreviary, ePrex,
   **Según tu Palabra** (destacada con el acento del sistema), Rezando
   Voy, Laudate — que se reproduce sola al entrar en la slide, tipo
   carrusel vertical: cada nombre entra desde abajo y se asienta antes
   de que entre el siguiente.
4. **03 — La solución** — mockup del móvil, con controles de vídeo
   nativos visibles (play/pausa, barra para rebobinar) para poder
   controlarlo en directo; los modos de estudio son el elemento
   protagonista — cuatro en total (Histórico, Cristológico, Etimológico,
   Pastoral) — con una animación tipo "ventana": cada uno aparece y se
   asienta antes de que aparezca el siguiente.
5. **03 — La solución** (biblia física) — mismo mockup fotográfico de la
   Biblia que la versión anterior del mazo, con un texto breve al lado.
6. **Primeras pruebas** — testimonios + QR, reutilizada tal cual (sin
   badge, para no repetir "03" una tercera vez seguida).
7. **04 — Propuesta de valor** — el recorrido de lectura (Leer → Entender
   → Reflexionar → Preguntar → Escribir → Compartir → Vivir) se reproduce
   solo, automáticamente, en cuanto se entra en la slide — sin que el
   usuario tenga que hacer clic para avanzar cada palabra. Cada palabra
   aparece con una temporización fija (~0,7s de intervalo); al terminar
   la secuencia completa, toda la fila crece a su tamaño final, grande y
   estático. Debajo, con menor protagonismo pero tipografía notablemente
   mayor que en la versión anterior, la comparación de tres: Hallow
   (oración), Magisterium (conocimiento/IA), y Según tu Palabra (Biblia +
   comunidad + herramientas + distribución) — esta última con el acento
   del sistema, para leerse como la opción destacada.
8. **05 — Cómo llegamos** — secuencia numerada de 5 pasos concretos (a
   quién nos dirigimos, cómo llegamos a ellos, qué les ofrecemos, cómo lo
   usan sus miembros, el objetivo de esta fase), reutilizando el mismo
   lenguaje visual de línea de tiempo del resto del mazo — línea vertical
   + punto — con número y un subtítulo esquemático (fragmentos cortos
   separados por punto medio, no oraciones completas) por paso.
9. **06 — El modelo** — las tres piezas que se complementan (App, Biblia
   física, Plataforma/comunidad) y, justo debajo de cada una, con el
   mismo peso visual que su descripción, quién paga por ella y cómo.
   Debajo de todo, sin jerarquía entre sí, el esqueleto del proceso
   operativo: Contacto → Acuerdo piloto → Configuración → Uso →
   Seguimiento → Pago → Transacciones.
10. **07 — La inversión** — badge + cifra (100.000€) apilados a la
    izquierda, justo encima del donut (que se queda en su sitio: un
    desglose proporcional real, con los porcentajes dados explícitamente,
    reutilizando el mismo lenguaje visual del anillo de "El problema").
    Leyenda en dos columnas (las partidas menores — gestoría, viajes,
    marketing, tecnología — agrupadas en una sola "Operación y
    lanzamiento" del 8%). A la derecha, tres tarjetas con lo que se
    consigue con esa inversión: producto en el mercado, empresa
    operativa, modelo validado.
11. **08 — El recorrido** — línea de tiempo horizontal protagonista
    (mismo componente que usaba antes también la slide "El plano"), 4
    hitos de izquierda a derecha, con la frase de apoyo centrada debajo.
12. **Cierre contemplativo** — sin badge, sin footer, centrado, mucho
    espacio en blanco. Dos citas, nada más.
13. **Portada (cierre)** — copia exacta de la slide 1: mismo marcado,
    mismo código, mismo bucle de palabras (incluido el nombre del
    proyecto debajo).

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
Biblias 4,5%, Constitución + legal 3,5%, y "Operación y lanzamiento" 8%
— esta última agrupa gestoría, viajes institucionales, marketing/ventas
y tecnología en una sola partida, para que la leyenda quepa en dos
columnas limpias. Los colores son pasos de opacidad de la propia paleta
navy más `--steel-dark` — no se añadió ningún color nuevo.

## Pendiente / decisiones a validar

- **Slide "El modelo" — qué monetiza cada pieza**: el mensaje no
  especificaba qué categoría de monetización corresponde a cada una de
  las tres piezas, así que hice la asociación más directa: App →
  Funciones premium con IA; Biblia física → Contrato diócesis/colegio;
  Plataforma/comunidad → Suscripción parroquia + Transacciones (cursos,
  retiros, donaciones). Dime si prefieres otra distribución.
- **Slide "El recorrido"**: el badge "08 — El recorrido" es una etiqueta
  propia (el mensaje original no especificaba el texto exacto del badge
  para esta slide) — cámbialo si prefieres otro.
