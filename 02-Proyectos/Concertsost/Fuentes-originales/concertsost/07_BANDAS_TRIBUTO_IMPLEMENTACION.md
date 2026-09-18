# CONCERTSOST — Bandas Tributo: implementación

Sección desarrollada siguiendo `CONCERTSOST_BANDAS_TRIBUTO_INSTRUCCIONES.md`, con la identidad visual ya cerrada del territorio Nodo (04_DECISIONS.md): negro `#000000` + verde `#40B72A`/`#236517`, Manrope + Karla + IBM Plex Mono, sistema gráfico de puntos y trayectos.

Actualizado con el catálogo real de 20 bandas, cuatro rondas de fotografía, la terminología definitiva, los costes reales de `GASTOS_BANDAS.xlsx`, columna "Banda original" en las tablas internas, clasificación Nacional/Internacional, enlaces directos a vídeo en las tarjetas, y el mensaje de marca en la cabecera (27/08/2026).

## Entregables

- **Web (catálogo + ficha):** artifact publicado — https://claude.ai/code/artifact/19b93632-2402-4bc3-9f39-b24d388c620b
- **Dossier PDF (6 páginas):** portada a página completa con mosaico de las 20 bandas (2×10, sin huecos, marcos anchos con las caras siempre visibles), catálogo "En exclusiva con CONCERTSOST" (4 bandas), catálogo "Ventaja CONCERTSOST" (9 bandas), catálogo "Selección CONCERTSOST" (7 bandas) — todas con la imagen a sangre completa en la tarjeta, sin franjas negras, burbuja Nacional/Internacional y enlace a vídeo cuando existe —, y dos páginas internas: "Costes reales" (estructura de coste + total por banda en exclusiva, con columna "Banda original") y "Condiciones internas" (notas generales de Ventaja y Selección, con columna "Banda original"). Enviado como `CONCERTSOST_Bandas_Tributo_Dossier.pdf`.

## Cambios de la última ronda (27/08/2026)

**1. Nueva banda: El Barrio, en Selección CONCERTSOST.** Añadida con fotografía facilitada por CONCERTSOST. Selección CONCERTSOST pasa de 6 a 7 bandas; el catálogo total pasa de 19 a 20. Se ha dado de alta con `tributeTo: 'El Barrio'` (mismo nombre que la banda comercial, ya que CONCERTSOST no distinguió un nombre de banda tributo distinto al del artista original, a diferencia de "Proud Tina" o "Stoned") y origen nacional (artista español) — a confirmar si el nombre comercial de la banda tributo es otro.

**2. Componentes corregidos.** CONCERTSOST facilitó el número de componentes que faltaba en tres bandas dadas de alta la ronda anterior: **Proud Tina** (Tina Turner) y **El Barrio** → 6 componentes; **Stoned** (Rolling Stones) y **Neon Collective** (Coldplay) → 5 componentes. Ya no aparecen como "Pendiente".

**3. Corrección del tributo de Ídem.** El tributo de **Ídem** pasa de "Manolo García" a **"El Último de la Fila y Manolo García"**, tal y como indicó CONCERTSOST (el repertorio de la banda cubre ambos proyectos).

**4. "Ver ficha" → "Ver vídeo" en las tarjetas, con enlace directo.** A petición de CONCERTSOST, cuando una banda tiene un vídeo de YouTube asignado, la tarjeta del catálogo (web y PDF) ahora dice **"Ver vídeo →"** y enlaza directamente a ese vídeo (se abre en pestaña nueva desde la web; en el PDF es un enlace real dentro del documento). CONCERTSOST facilitó vídeos para 16 de las 20 bandas — se han asociado por coincidencia de artista/banda original:

| Banda tributo | Banda original | Vídeo |
|---|---|---|
| Ultrarumba | Estopa | youtu.be/VzaupaC8B9w |
| Fábula | Mecano | youtu.be/8e385Xb--rk |
| Euforia | Alaska | youtu.be/HCdArZ9CbmI |
| Queen Universe | Queen | youtu.be/rf-T_6movKg |
| La Esencia del Loco | El Canto del Loco | youtu.be/CXPv-QB131M |
| El Despertar del Silencio | Héroes del Silencio | youtu.be/slvH-3TAlF4 |
| Ídem | El Último de la Fila y Manolo García | youtu.be/WyWbR36-Zww |
| Whisky Barato | Fito & Fitipaldis | youtu.be/-P2_wmSIixs |
| Reina del Pop | La Oreja de Van Gogh | youtu.be/-Sep2KymEXE |
| Midnight Riders | Bon Jovi | youtu.be/2JlErAOcNXc |
| U2 Band | U2 | youtu.be/tuboieJ4A9g |
| The Honey's | ABBA | youtu.be/84Erf0gSw9o |
| El Barrio | El Barrio | youtu.be/74108goQ0BI |
| Proud Tina | Tina Turner | youtu.be/VzaupaC8B9w |
| Stoned | Rolling Stones | youtu.be/R6vEaJvVN2g |
| Neon Collective | Coldplay | youtu.be/SZc_4TIFrMI |

Sin vídeo asignado (siguen con "Ver ficha →", que lleva a la ficha de la web): **RKid**, **Rock Legends**, **Lobos**, **Blisters**.

Dos cosas a revisar en la lista que envió CONCERTSOST, porque parecen no intencionadas y no se han corregido por iniciativa propia (no inventar datos):
- El enlace para **Estopa/Ultrarumba** y el enlace para **Tina Turner/Proud Tina** son idénticos (`youtu.be/VzaupaC8B9w`) — probablemente uno de los dos está duplicado por error.
- Se enviaron **dos enlaces distintos para "Bon Jovi"** (`youtu.be/2JlErAOcNXc` y `youtu.be/sgYGGQDMxkE`), pero solo hay una banda tributo a Bon Jovi (Midnight Riders). Se ha usado el primero; el segundo ha quedado sin usar.

## Cambios de la ronda anterior (27/08/2026, altas + nacional/internacional)

**1. Tres bandas nuevas en Selección CONCERTSOST.** A petición de CONCERTSOST se añadieron, con fotografía del artista/banda original facilitada por ellos: **Proud Tina** (tributo a Tina Turner), **Stoned** (tributo a Rolling Stones), **Neon Collective** (tributo a Coldplay).

Se adjuntó una cuarta imagen (hombre con sombrero fedora, pañuelo de lunares, tatuaje de estrella en la muñeca, cantando con micrófono, luz azul de escenario) que **no se ha asignado a ninguna banda**: no coincidía visualmente con Tina Turner, Rolling Stones ni Coldplay, los tres tributos nombrados explícitamente en ese momento. Sigue sin usar — pendiente de que CONCERTSOST indique a qué banda/artista corresponde.

**2. Clasificación Nacional / Internacional.** Se añadió un campo `origin` (`'nacional'` | `'internacional'`) a cada banda, visible como una pequeña burbuja discreta en la esquina superior derecha de cada tarjeta (opuesta a la burbuja de categoría, que sigue en la esquina superior izquierda), tanto en la web como en el PDF. Dentro de cada categoría (Exclusiva / Ventaja / Selección), las tarjetas se ordenan primero las nacionales y después las internacionales.

La clasificación nacional/internacional de las bandas ya existentes se ha inferido a partir de la nacionalidad conocida del artista/banda original al que rinden tributo (dato de dominio público, no facilitado explícitamente por CONCERTSOST) — conviene que CONCERTSOST lo revise. Un caso dudoso en particular: **Rock Legends** tiene como tributo "Rock (varios artistas)", sin nacionalidad concreta asociada; se ha marcado como internacional por defecto, pero es una suposición propia, no un dato confirmado.

**3. Columna "Banda original" en las tablas internas de coste.** Las dos páginas de uso interno ("Costes reales" y "Condiciones internas") ya incluían el nombre de la banda tributo y sus componentes; ahora cada fila también muestra el nombre del artista/banda original (ej. "Ultrarumba — Estopa").

**4. Portada — eliminado texto redundante.** Se quitó de la portada del PDF la frase "Catálogo compacto, fichas claras y datos de coste gestionados aparte, de forma interna".

**5. Fix técnico del mosaico de portada.** Al ampliar el mosaico las últimas filas no aparecían: por defecto, una fila de cuadrícula con `1fr` no se reduce por debajo del tamaño mínimo de su contenido, así que las filas de más abajo se salían del área de la portada y quedaban cortadas por el `overflow: hidden` de la página. Se corrigió forzando `minmax(0, 1fr)` en filas y columnas del mosaico (y `min-height: 0` en el contenedor y en las imágenes).

## Cambios de rondas anteriores (27/08/2026, mensaje de cabecera + ajuste fino)

**Nueva jerarquía del bloque bajo "Bandas Tributo.".** El mensaje de marca ocupa ahora el lugar principal bajo el título:

> **Experiencia que se escucha.**
> Desde 2007 creamos y desarrollamos bandas tributo con una premisa clara: ofrecer espectáculos excepcionales, con artistas de primer nivel y una alta exigencia de calidad. Nuestra experiencia nos permite seleccionar y desarrollar propuestas que funcionan sobre el escenario y responden a las necesidades de cada programación.

El texto descriptivo original ("Cartera de propuestas musicales de bandas tributo lista para presentar...") queda relegado más abajo, en gris tenue, con función puramente informativa. Aplicado igual en la web y en la portada del PDF.

**Mosaico de portada — marcos anchos, caras siempre visibles** (cuadrícula 2 columnas × N filas en vez de 4×4, para que la proporción del marco se acerque al 4:3 de las fotos). **Tarjetas del catálogo a sangre completa, sin franjas negras** (marcos ajustados al 4:3 de origen + `object-fit: cover`). **RKit → RKid** (nombre correcto según `GASTOS_BANDAS.xlsx`). **Notas de condiciones generalizadas por categoría** en vez de ligadas a una banda concreta.

## Terminología de clasificación (definitiva)

- **★ Exclusiva** — grupo "En exclusiva con CONCERTSOST". Descripción: "Propuestas que solo encontrarás en la selección de CONCERTSOST."
- **● Ventaja CONCERTSOST** (antes "Buena relación" / "Muy buena relación") — grupo "Ventaja CONCERTSOST". Descripción: "Condiciones preferentes CONCERTSOST." Nota general (uso interno): "Trato ventajoso con PATOS / CONCERTSOST — mejores condiciones, mayor flexibilidad. Cachés similares a los de exclusiva — verificar siempre al confirmar fecha."
- **Selección CONCERTSOST** — sin nota descriptiva pública. Nota general (uso interno): "Contacto con banda y recomendación, pero mayor caché / condiciones menos flexibles. Cachés indeterminados — recomendación mínima de 3.000 € + gastos."
- **Nacional / Internacional** — burbuja discreta en cada tarjeta (esquina opuesta a la de categoría), según la nacionalidad del artista/banda original.
- **Ver vídeo / Ver ficha** — la tarjeta enlaza al vídeo de YouTube si CONCERTSOST facilitó uno para esa banda; si no, enlaza a la ficha (web).

Ni la web ni el PDF muestran el número total de bandas del catálogo en la portada/cabecera; el contador por sección sigue visible junto a cada título de grupo.

## Catálogo actual (20 bandas)

**★ En exclusiva con CONCERTSOST:** Ultrarumba (Estopa, 7, nacional), Fábula (Mecano, 6, nacional), Euforia (Alaska, 5, nacional), Queen Universe (Queen, 5, internacional).

**● Ventaja CONCERTSOST:** La Esencia del Loco (El Canto del Loco, 5, nacional), El Despertar del Silencio (Héroes del Silencio, 4, nacional), Ídem (El Último de la Fila y Manolo García, 5, nacional), Whisky Barato (Fito & Fitipaldis, 6, nacional), Reina del Pop (La Oreja de Van Gogh, 5, nacional), RKid (Oasis, 4, internacional), Midnight Riders (Bon Jovi, 4, internacional), U2 Band (U2, 4, internacional), Rock Legends (Rock varios artistas, 6, internacional — clasificación asumida, a confirmar).

**Selección CONCERTSOST:** Lobos (Leiva, 5, nacional), El Barrio (El Barrio, 6, nacional), The Honey's (ABBA, 6, internacional), Blisters (The Beatles, 5, internacional), Proud Tina (Tina Turner, 6, internacional), Stoned (Rolling Stones, 5, internacional), Neon Collective (Coldplay, 5, internacional).

Ningún nombre, artista, número de componentes, categoría, origen, vídeo o coste es inventado salvo donde se indica expresamente como suposición propia (Rock Legends → internacional; el origen nacional de El Barrio, inferido de la nacionalidad del artista): son los datos que facilitó CONCERTSOST (chat + `GASTOS_BANDAS.xlsx` + imágenes + lista de vídeos). Sigue pendiente (con placeholder): presskit y links de interés de las 20 bandas; el coste real cerrado de las 16 bandas de Ventaja/Selección; vídeo de RKid, Rock Legends, Lobos y Blisters; y la identificación de la imagen del hombre con sombrero fedora que sigue sin usar.

## Costes reales (uso interno, GASTOS_BANDAS.xlsx)

*Estructura de coste (exclusiva), por paquete según tamaño de formación:*

| Concepto | Paquete 5+1 (bandas de 5) | Paquete 6/7+1 (bandas de 6-7) |
|---|---|---|
| Músicos / road | 250 €/persona | 250 €/persona |
| Caché base | 1.500 € | 2.000 € |
| Transporte (24h) | 250 € | 250 € |
| Gasolina (ida-vuelta, radio ~150 km) | 100 € | 100 € |
| Dietas (por día) | 180 € | 210 € |
| Hotel (media 40 €/persona) | 250 € | 320 € |
| Oficina | Pendiente de datos | Pendiente de datos |
| **Total** | **2.280 €** | **2.880 €** |

*Coste total estimado por banda en exclusiva* (paquete asignado según componentes, con banda original): Ultrarumba/Estopa 2.880 €, Fábula/Mecano 2.880 €, Euforia/Alaska 2.280 €, Queen Universe/Queen 2.280 €.

Ninguna de las 16 bandas de Ventaja/Selección tiene un coste real cerrado en el Excel, así que sus celdas de coste siguen en "Pendiente de datos" a propósito — solo llevan las notas generales de categoría (ver arriba). Esto vive únicamente en las dos páginas internas del PDF, nunca en la web ni en el catálogo comercial.

## Fotografías — tratamiento

CONCERTSOST facilitó las fotografías, una por banda. **Son imágenes del artista/banda original**, no de la formación tributo — sirven como referencia visual de "a quién rinde tributo" más que como foto de la banda tributo en sí. Vale la pena tenerlo en cuenta de cara a derechos de imagen si el dossier circula fuera de un uso interno/comercial directo — decisión de CONCERTSOST, no algo que resolver aquí, pero queda anotado.

Tratamiento aplicado a todas, igual en web y PDF: recorte a 4:3 con sesgo superior, duotono negro-verde muy apagado (16% de color original reintroducido), embebidas en `band_photos/` (PDF) y como base64 (web). En las tarjetas se muestran a sangre completa (`object-fit: cover`) sobre marcos ajustados al 4:3 de origen. Portada del PDF: mosaico 2×10 (20 fotos, sin huecos) con marcos anchos que dejan ver la cara completa, recorte diagonal de marca, a página completa.

Cuando CONCERTSOST facilite fotos reales de las formaciones tributo, sustituir el campo `image` de cada banda — el resto del sistema no cambia.

## Por qué son un archivo independiente y no un cambio directo sobre la web publicada

Esta sesión no tuvo acceso de lectura al HTML ya publicado de concertsost.com (bloqueo de red del entorno hacia el dominio del artifact). Por eso la sección se construyó como pieza autocontenida, reutilizando los tokens de marca ya documentados, en vez de editar el archivo original a ciegas.

Para integrarla como sección real de la web: mover el `<div class="bt-app">`, el `<style>` y el `<script>` del archivo al HTML principal, reutilizando las fuentes que ya carga esa página, y añadir un ancla "Bandas Tributo" al nav existente. Todas las clases usan el prefijo `bt-` para no chocar con el resto del sitio.

## Fuentes en el PDF (pendiente de sustituir)

El entorno donde se generó el PDF no tuvo acceso de red a Google Fonts, así que el dossier usa sustitutos tipográficos ya instalados en el sistema mientras no se disponga de los archivos reales:

| Rol de marca | Usado en el PDF |
|---|---|
| Manrope (títulos) | Liberation Sans |
| Karla (texto) | Carlito |
| IBM Plex Mono (datos/etiquetas) | DejaVu Sans Mono |

Colores, retícula y jerarquía sí son los definitivos. En cuanto se pueda acceder a los .ttf/.woff2 reales de Manrope/Karla/IBM Plex Mono, regenerar el PDF sustituyendo solo las variables de fuente. La web sí carga las fuentes de marca reales desde Google Fonts.

## Esquema de datos (escalabilidad)

Añadir, quitar o modificar una banda = editar un objeto en `TRIBUTE_BANDS` en el `<script>` del artifact web (y su equivalente `BANDS` en dossier.html para el PDF, con `video` como campo simple en vez de array `videos`). No se toca HTML, CSS ni lógica de render; el catálogo se reagrupa y reordena solo.

```js
{
  slug: 'texto-unico-sin-espacios',
  name: 'Nombre comercial de la banda tributo',
  tributeTo: 'Nombre de la banda/artista original',
  tier: 'exclusiva' | 'relacion' | null,   // 'relacion' se muestra como ● Ventaja CONCERTSOST
  origin: 'nacional' | 'internacional',    // burbuja discreta, ordena las tarjetas dentro de cada categoría
  members: 5,                 // SOLO el número de integrantes, o null si falta el dato
  image: 'data:image/jpeg;base64,...' | null, // o una URL; null -> marcador gráfico de marca
  presskit: 'Texto de presentación proporcionado por CONCERTSOST.' | null,
  videos: [{ label: 'Vídeo', url: 'https://youtube.com/...' }],  // el primero se usa como "Ver vídeo" en la tarjeta; si está vacío, la tarjeta enlaza a la ficha
  links: [{ label: 'Instagram', url: 'https://...' }],
}
```

Los costes reales **no existen como campo en este esquema**, a propósito — nunca deben llegar a la web ni al catálogo comercial. Viven únicamente en las dos páginas internas del PDF (estructura de coste + condiciones, con columna "Banda original"), que se amplían banda a banda cuando CONCERTSOST facilite más datos económicos.
