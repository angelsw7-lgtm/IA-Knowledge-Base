# CONCERTSOST — DECISIONES

## Nombre de marca
**Concertsost** (no "Concertost"). Corregido en todos los documentos y entregables.

## Confirmado — Identidad visual (cerrada)
- Concertsost es una marca B2B, siempre vinculada al contexto de eventos.
- Sus territorios incluyen alianzas, nuevos proyectos, patrocinios, turismo + música, innovación, sostenibilidad, networking, reuniones y nuevos formatos.
- La primera fase es identidad visual + web. ChatGPT marca las pautas estratégicas/creativas y Claude ejecuta.
- **Territorio visual: Nodo** (de los 3 explorados: Nodo, Plaza, Señal — ver 06_VISUAL_TERRITORIES.md).
- **Logotipo definitivo**: wordmark "concertsost", en 4 versiones — color sobre claro (concert negro + sost verde), color sobre oscuro (concert blanco + sost verde), monocromo negro, monocromo blanco. Archivo cerrado: no se recompone en otra tipografía ni se recolorea.
- **Paleta**: negro #000000 y verde #40B72A (extraídos del logotipo) + derivados tonales — verde profundo #236517, verde medio #A9DF9F, verde lavado #ECF8EA, gris texto #565B54.
- **Isotipo**: el mismo motivo de puntos conectados por trayectos de extremos redondeados y opacidad decreciente del sistema gráfico de Nodo, llevado a marca independiente.
- **Tipografía**: Manrope (titulares) + Karla (texto) + IBM Plex Mono (datos/etiquetas).
- **Sistema gráfico**: puntos y trayectos de conexión con terminales redondeadas, en verde sobre negro o blanco.
- **Dirección fotográfica**: fotografía real de negocio/eventos, recorte en diagonal, duotono negro/verde sutil. Sin clichés de concierto.
- **Composición**: retícula basada en el ángulo del sistema gráfico, espaciado en base 8px, un único acento verde por sección.
- **Reglas de uso**: área de seguridad = altura de la "o" minúscula alrededor del logo; tamaño mínimo 90px (wordmark) / 16px (isotipo solo); no recolorear, no distorsionar, no usar sobre fondos de bajo contraste, no recomponer en otra tipografía.

Documentado con ejemplos visuales: https://claude.ai/code/artifact/7c8b7393-47af-4d6d-88f2-22d8076265e7

## Confirmado — Web (v3, aprobada como versión de trabajo)
- Página única con navegación por anclas: Home (hero) → Qué es → Qué hacemos → Proyectos y oportunidades → Ecosistema → Contacto.
- Dirección visual estilo "Apple": red de nodos en 3D animada (canvas, sin librerías externas) en el hero; fondo con transición gradual de color entre todas las secciones (blanco → verde → blanco → negro → blanco), sin cortes duros; tarjetas con efecto cristal (glass morphism); inclinación 3D al pasar el ratón; botones interactivos con brillo, elevación y pulsación; dos imágenes de referencia abstractas en negro/verde, marcadas como referencia (no fotografía real).
- Botón "Hablemos" y CTAs de contacto: texto blanco sobre verde profundo #236517 (contraste de accesibilidad), hover a negro.
- Contacto con emails reales: `info@concertsost.com` (información general) y `comunicacion@concertsost.com` (comunicación y prensa).
- Responsive (nav con menú móvil), animaciones respetan `prefers-reduced-motion`, estados de foco visibles.
- El resto del contenido comercial sigue siendo placeholder claramente marcado: proyectos "[Nombre del proyecto]" con etiqueta "Próximamente", logos de partners como bloques "Partner".

Publicada en: https://claude.ai/code/artifact/70e37d8b-f69d-4af5-b60f-a0d10419be23

## Pase de consistencia (25/08/2026)
A petición del cliente ("podemos actualizar todos los archivos?") se revisaron los 3 entregables HTML y los 7 documentos del proyecto para verificar que todos reflejan las últimas decisiones:
- Nombre de marca "Concertsost" verificado correcto en los tres HTML (`territorios.html`, `identidad-nodo.html`, `web/index.html`) y en los 7 documentos del proyecto — sin restos de "Concertost".
- **Corregido**: en `identidad-nodo.html`, la sección "06 · Dirección web" tenía un botón de mockup (`.mockup-cta`) que aún usaba verde brillante `#40B72A` con texto blanco — la misma combinación de bajo contraste (~2.61) descartada más tarde para la web real. Actualizado a verde profundo `#236517` para que el documento de identidad sea coherente con la implementación real.
- `territorios.html` revisado: sin botones con la combinación de bajo contraste, nombre de marca correcto. Se mantiene como referencia histórica de las 3 direcciones exploradas (paleta ámbar/verde original de "Nodo", ya sustituida).
- Los tres artifacts se republicaron para reflejar estos cambios en sus URLs ya existentes.

## Estado
**v3 (25/08/2026):** aprobada como base de trabajo, con placeholders claramente marcados para proyectos y partners.

**v4 (15/09/2026):** la web incorpora ya vídeo de portada real, fotografía real en "Qué es", los 3 proyectos reales y los 6 logos de partners reales — ver detalle en la actualización de abajo. El botón "Hablemos" del nav, que había quedado ilegible por un bug de CSS, está corregido. Existe además un tema de WordPress instalable (cada sección como página independiente) como entregable adicional. Cuando se retome, revisar primero este documento y el artifact de la web antes de seguir iterando.

## Actualización (15/09/2026) — vídeo de portada, contenido real y tema WordPress
- **Nueva sección de vídeo a pantalla completa** como primer bloque de la home: vídeo del cliente (`VIDEO-WEB-.mp4`, original 1080p/67s/55MB) comprimido a ~12,7MB (720p, 25fps, sin audio) para que cargue rápido; capa oscura negro/verde encima para legibilidad; titular superpuesto "El punto de encuentro que mueve el ecosistema de eventos."; indicador de scroll animado. Respeta `prefers-reduced-motion` (pausa el vídeo).
- **Hero de texto** (la sección que sigue al vídeo) actualizado: "De la idea a la alianza: bienvenido al ecosistema Concertsost."
- **Contenido comercial real incorporado**, sustituyendo los placeholders mencionados antes en "Pendiente":
  - "Qué es": foto de referencia sustituida por fotografía real de un concierto de Hombres G.
  - "Proyectos": los 3 cuadros "[Nombre del proyecto] / Próximamente" sustituidos por SkyFest Benidorm (gestión y asesoramiento), Hombres G en Castellón (producción y gestión íntegra del concierto) y Vinal Fest (producción y gestión íntegra del festival), cada uno con foto real.
  - "Ecosistema": los 6 bloques "Partner" sustituidos por los logotipos reales (en blanco) de Ayuntamiento de Castelló, Babalú, BCDME, SkyFest, Producciones Patos y un sexto logo (`LOGO2.png`, pendiente de confirmar el nombre del partner).
- **Bug corregido**: el botón "Hablemos" del nav era ilegible (texto negro sobre su propio fondo negro) por un problema de especificidad CSS (`.nav-links a` pisaba el color blanco de `.nav-cta`). Corregido y alineado con lo ya decidido arriba: verde profundo `#236517` por defecto, hover a negro.
- **Añadido enlace a Instagram** (icono en el nav + texto en el footer): https://www.instagram.com/concert.sost
- Revisado con capturas en escritorio y móvil (incluyendo el menú móvil desplegado) tras los cambios.
- Publicada en el mismo artifact ya existente: https://claude.ai/artifact/1T3pZt2hNKMJ3Bek1J7u1P
- **Nuevo entregable**: tema de WordPress instalable (`concertsost-theme.zip`) donde cada sección (Qué es, Qué hacemos, Proyectos, Ecosistema, Contacto) es una página independiente con su propia plantilla; la portada combina el vídeo + el hero de texto. Al activar el tema se crean automáticamente las 5 páginas. Pendiente de instalar en un hosting real.

## Pendiente para la versión definitiva
- Versión vectorial (SVG) de logotipo e isotipo — los archivos actuales son PNG de baja resolución (~534×145px).
- Confirmar el nombre del partner correspondiente al logo `LOGO2.png` (ecosistema).
- Instalar el tema de WordPress en el hosting definitivo de concertsost.com.
- Cualquier ajuste adicional de diseño o estructura que el cliente pida en la siguiente vuelta.

## Assets previos (no usados como base)
- `ISOTIPOCOLOR.png`: isotipo de árbol con notas musicales y hoja. No usado como referencia porque el brief pide evitar iconografía musical literal.
