# Identidad visual y web — Sabor a Música

Fuente: proyecto real de construcción de la landing `patosagencia.com/sabor-a-musica/`, incluida su evolución a través de varias iteraciones de feedback directo de Ángel. Esta es información sólida porque son decisiones de diseño realmente tomadas y verificadas en la web publicada, no texto del dossier.

## Activos de marca — logotipo

Existen dos versiones oficiales del logotipo, ambas en formato wordmark manuscrito/script "sabor a Música" con una nota musical en dorado como elemento gráfico de acento:

- **Versión negra** (para fondos claros): `https://www.patosagencia.com/wp-content/uploads/2026/07/LOGO-SAM-NEGRO.png`
- **Versión blanca** (para fondos oscuros): `https://www.patosagencia.com/wp-content/uploads/2026/07/LOGO-SAM-BLANCO.png`

Formato original de los archivos: PNG, 1080×1080px, fondo transparente.

### Activos que NO son de Sabor a Música — aviso importante

Durante este proyecto aparecieron en la carpeta de conocimiento del proyecto varios archivos que **no son** el logotipo de Sabor a Música, aunque estaban en la misma carpeta:

- Dos wordmarks "concertsost" (una en negro, otra bicolor negro/verde).
- Un icono de árbol con notas musicales y hojas, también de la marca ConcertSost.

Se confirmó independientemente (sesión "HTML firma de email" en este mismo entorno) que ConcertSost es una marca real y separada, con dominio propio `concertsost.com`. Ver `19_ENTIDADES_RELACIONADAS.md`. **No usar estos archivos como logotipo de Sabor a Música bajo ninguna circunstancia.**

## Sistema tipográfico

- **Display / titulares**: Fraunces (serif editorial, variable, con cursivas elegantes) — vía Google Fonts.
- **Cuerpo de texto / UI**: Inter (sans-serif) — vía Google Fonts.

Criterio de elección: buscar un carácter "editorial, premium, muy contemporáneo" (brief textual de Ángel), evitando tipografías corporativas genéricas.

## Paleta de color

| Color | Valor | Uso |
|---|---|---|
| Blanco cálido / papel | `#fbfaf7` | Fondo base en estado "claro" |
| Negro cálido / tinta | `#0a0908` (fondo) / `#141210` (texto) | Fondo/texto en estado "oscuro" |
| Dorado | `#c69a4a` | Acento de marca — tomado directamente del color de la nota musical del logotipo |
| Dorado suave | `#d9b876` | Variante clara del acento, para texto sobre fondo oscuro |
| **Tercero (cognac/burdeos)** | `#3a231b` | Tercer estado de fondo, añadido en la tercera iteración a petición explícita de Ángel — ver evolución más abajo |

El dorado (`#c69a4a`) es el único color de acento verdadero de la marca en la web: se tomó por muestreo directo del color de la nota musical dorada dentro del propio logotipo, no es una elección arbitraria.

## Estructura de la web

Página única de scroll (landing de una sola página), con 12 bloques en este orden fijo, calcado literalmente a la estructura y numeración del dossier:

1. Apertura (hero)
2. 01 · Quiénes somos
3. 02 · Nuestra visión
4. 03 · Qué hacemos
5. 04 · Nuestro método
6. 05 · Nuestra diferencia
7. 06 · Nuestro ecosistema
8. 07 · Nuestros pilares
9. 08 · Experiencias
10. 09 · Para quién
11. 10 · Nuestra filosofía
12. Cierre

Cada sección numerada muestra su "eyebrow" (etiqueta pequeña superior) con el número y título tal cual aparecen en el dossier (p. ej. "01 · Quiénes somos").

## Criterio de diseño — brief original de Ángel (textual)

Este es el brief de dirección de arte tal como se recibió, y ha sido la referencia constante durante todo el proyecto:

- Estética editorial, premium y muy contemporánea.
- Base minimalista blanca, luminosa y aireada.
- Transiciones entre secciones con transformación de luz (fondo de blanco a negro, tipografía invertida a blanco).
- Halos, reflejos, gradientes suaves, destellos controlados, volumetrías 3D abstractas — sofisticado, no recargado.
- Elementos gráficos abstractos relacionados con sonido, ritmo, copa, territorio y experiencia.
- Sin imágenes de stock genéricas.
- Logotipo sutil: abre y cierra la web, sin ser un elemento dominante.
- Responsive, con movimiento fluido, sobrio y elegante.

## Tratamiento del logotipo en la web (decisión vigente)

- **Apertura (hero)**: el logotipo es el único elemento de título — no hay texto "SABOR A MÚSICA" en H1. Tamaño responsive `clamp(190px, 220px + 10vw, 420px)`, lo que da aproximadamente 190–260px en móvil y 280–420px en escritorio. Debajo del logo: el claim "Experiencias que conectan personas, marcas y territorio." y la firma "Powered by Patos Producciones".
- **Cierre**: mismo logotipo, tratamiento más sutil — tamaño `clamp(120px, 130px + 6vw, 230px)`, sin texto adicional (para no repetir el nombre de la marca donde el logo ya la comunica).
- **Marca de agua persistente**: un pequeño logotipo fijo en la esquina inferior derecha (~56px), visible solo después de hacer scroll más allá del hero, que hace crossfade automático entre la versión negra y blanca según el fondo del momento. Es la única repetición adicional del logo, deliberadamente discreta.

### Evolución — versión anterior superada

La primera versión de la web incluía un H1 con el texto "SABOR A MÚSICA" además de un logotipo pequeño (~120px) junto a él. Ángel pidió explícitamente eliminar el texto y que el logotipo pasara a ser el único título visual, con mayor presencia. **Esta es la decisión vigente; la versión con H1 de texto está descartada.**

## Motor de transición de color (fondo claro ↔ oscuro)

Sistema técnico, documentado porque condiciona cualquier cambio futuro de contenido o estructura de la web:

- Variable CSS `--tone` (0 = blanco, 50 = tercero/cognac, 100 = negro), animada de forma nativa vía `@property` + `color-mix()`, con una transición suave de ~1.3s.
- Un script mide la posición de scroll y el centro vertical real de cada sección (`data-tone`) para interpolar el valor de `--tone` de forma continua, en vez de saltar de golpe.
- El color de texto (`--fg`), el color de texto secundario (`--fg-muted`) y el color de líneas/bordes (`--line`) están ligados a la misma variable, por lo que se invierten automáticamente en sincronía con el fondo.

### Evolución — versiones anteriores superadas

1. **V1**: franjas de degradado independientes (`<div class="transition">`) insertadas entre cada sección, con un salto de blanco a negro dentro de cada franja. Feedback de Ángel: "se percibían como bloques separados", "cortes". **Descartada.**
2. **V2**: se eliminaron las franjas y se pasó a un sistema continuo de una sola variable `--tone` binaria (0/100) interpolada por sección, pero alternando en casi todas las secciones. Feedback de Ángel: las transiciones eran demasiado frecuentes y algunas secciones mostraban cortes de fondo (causados por `overflow:hidden` combinado con desenfoque, un artefacto de renderizado). **Descartada.**
3. **V3 (vigente)**: la que se describe arriba — fases de fondo constante de 2–3 secciones seguidas antes de cada cambio, tercer color intermedio (cognac) añadido como estado real (no solo un punto de paso matemático), y se retiró el `overflow:hidden` por sección para eliminar los cortes de renderizado.

### Secuencia de tono vigente (fase por fase)

| Fase | Secciones | Tono |
|---|---|---|
| 1 | Apertura + Quiénes somos | 0 (blanco) |
| 2 | Visión + Qué hacemos + Método | 100 (negro) |
| 3 | Diferencia + Ecosistema | 50 (tercero/cognac) |
| 4 | Pilares + Experiencias | 0 (blanco) |
| 5 | Para quién + Filosofía | 100 (negro) |
| 6 | Cierre | 0 (blanco) |

## Tratamiento de la sección "08 · Experiencias" (sin fotografía real)

No existe ninguna fotografía real de eventos de Sabor a Música en ninguna de las fuentes disponibles (ni en el dossier, ni en los adjuntos del proyecto). Ante la instrucción de "evitar imágenes de stock genéricas" y no tener material propio, se optó por composiciones abstractas 3D/luz en vez de fotografía de stock:

| Experiencia | Tratamiento visual |
|---|---|
| Show Must Go On | Forma orgánica ámbar/burdeos con motivo de arco de bodega, tono cálido de vino |
| Slow Sessions | Forma orgánica verde-dorado con motivo de rama/naturaleza |
| Experiencias Corporativas | Forma en grafito/cromo con anillos concéntricos |
| Activaciones de Marca | Forma en dorado con destello radiante |

Esto queda marcado como **placeholder pendiente de sustitución** por fotografía real cuando exista — se lo comunicó explícitamente a Ángel durante el proyecto.

## Otros recursos visuales del sistema

- Textura de grano/ruido sutil superpuesta a toda la web (SVG de turbulencia, muy baja opacidad).
- Parallax ligero en algunos halos y elementos de disco (velocidades bajas, movimiento sutil ligado al scroll).
- Iconos lineales abstractos propios para cada uno de los seis pilares (sección "07 · Nuestros pilares").
- Anillo/"hub" decorativo detrás del listado de nodos de "06 · Nuestro ecosistema" para sugerir un sistema conectado.

## Incidencia de despliegue y solución (histórico técnico)

La primera publicación en `patosagencia.com/sabor-a-musica/` se veía sin ningún estilo (texto plano, sin tipografía, colores ni animaciones). Diagnóstico: la web está construida en WordPress + Elementor, y el contenido se había pegado en un widget de texto estándar, que sanea automáticamente el contenido y elimina las etiquetas `<style>` y `<script>`. Solución indicada: usar el widget "HTML"/Código personalizado de Elementor (no sanea el contenido), o alternativamente alojar el archivo como página independiente e incrustarla con un `<iframe>`. Confirmado resuelto el 27 de agosto de 2026 según verificación directa de la URL pública.

## Formato de entrega técnico

Archivo HTML único autocontenido (CSS y JS inline en el mismo archivo), sin dependencias externas salvo Google Fonts. Sin imágenes locales — todas las imágenes (los dos logotipos) se referencian por URL absoluta ya alojada en el servidor del cliente.
