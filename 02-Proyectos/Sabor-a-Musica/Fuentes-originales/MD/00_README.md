# Base de conocimiento — Sabor a Música

## Qué es esta biblioteca

Documentación estructurada de la marca **Sabor a Música**, pensada para poder entregarse a Claude (o a cualquier otra IA) en una conversación nueva y que esta entienda la marca en profundidad sin necesitar el histórico de conversaciones original.

No es una presentación ni un resumen de marketing. Es documentación interna: precisa, sin relleno, organizada por temas, con las fuentes y el nivel de confianza de cada dato indicados explícitamente.

## Qué es Sabor a Música

Sabor a Música es la marca de experiencias de **Patos Producciones**, promotora musical con más de 25 años (dossier también usa "más de dos décadas") de trayectoria en producción de conciertos, festivales y eventos. Traslada ese conocimiento al mundo de las marcas, diseñando experiencias donde música, gastronomía, vino, cultura y territorio se combinan para crear momentos memorables para empresas, bodegas, hoteles, instituciones y otras organizaciones.

Detalle completo en `01_IDENTIDAD_DE_MARCA.md`.

## De dónde sale esta información — léelo antes de usar la biblioteca

Esto es importante y hay que decirlo con claridad: esta biblioteca **no** se ha construido a partir de un histórico extenso de muchas conversaciones sobre Sabor a Música. Se ha construido a partir de dos fuentes reales, y solo dos:

1. **El dossier oficial de la marca** (`DOSSIER SAM.md`), el documento fuente que define el contenido de marca: quiénes somos, visión, qué hacemos, método, diferencia, ecosistema, pilares, experiencias, para quién y filosofía.
2. **El proyecto de la landing web de Sabor a Música** (esta misma conversación y su continuación), donde se tomaron decisiones reales de diseño, estructura, tono visual y comunicación al construir `patosagencia.com/sabor-a-musica/`.

Antes de generar esta biblioteca se revisaron las demás sesiones de trabajo disponibles en este entorno. Se encontraron cuatro:

- **Manual de identidad visual** → es sobre **Fusion Town**, no sobre Sabor a Música. Excluida.
- **Fusion Town landing page design** → es sobre **Fusion Town**, no sobre Sabor a Música. Excluida.
- **HTML firma de email** → es sobre **ConcertSost** (firma de comunicacion@concertsost.com). Excluida, salvo la mención de que esa marca existe y tiene dominio propio (ver `19_ENTIDADES_RELACIONADAS.md`).
- **Plan de pago límite** → pregunta sobre límites de uso de la suscripción a Claude. Sin relación con la marca. Excluida.

No se encontró ningún otro documento, conversación o archivo adicional sobre Sabor a Música más allá del dossier y el proyecto de la web. Si en realidad existe más trabajo previo sobre la marca (reuniones, borradores, otras conversaciones no accesibles desde este entorno), **no está reflejado aquí** y conviene añadirlo a mano o pegarlo en una futura conversación para ampliar esta base.

Esto significa que, allí donde la plantilla de esta biblioteca pide información que la conversación original daba por hecho que existía (por ejemplo, bandas tributo, casos de cliente reales, argumentario de objeciones, política de sostenibilidad detallada), y esa información no aparece ni en el dossier ni en el proyecto de la web, el archivo correspondiente lo marca explícitamente como `PENDIENTE DE DEFINIR` o `INFORMACIÓN NO CONFIRMADA` en lugar de inventarlo.

## Cómo están organizados los archivos

### Estratégicos (marca, no proyecto)

| Archivo | Contenido |
|---|---|
| `01_IDENTIDAD_DE_MARCA.md` | Qué es, origen, relación con Patos Producciones, propósito, visión, valores |
| `02_POSICIONAMIENTO.md` | Cómo se quiere que se perciba la marca, diferenciación |
| `03_PROPUESTA_COMERCIAL.md` | Argumentos de venta, qué compra el cliente |
| `04_SERVICIOS_Y_FORMATOS.md` | Catálogo de formatos de experiencia |
| `05_METODOLOGIA_Y_PRODUCCION.md` | Cómo trabaja Sabor a Música, de la idea al evento |
| `06_PUBLICOS_Y_CLIENTES.md` | Mapa de clientes potenciales |
| `07_COMUNICACION_Y_TONO.md` | Tono de voz, patrones de escritura de marca |
| `08_IDENTIDAD_VISUAL_Y_WEB.md` | Identidad visual, sistema de diseño de la web, decisiones tomadas y su evolución |

### Proyectos concretos

| Archivo | Contenido |
|---|---|
| `09_EXPERIENCIAS_Y_PROYECTOS.md` | Índice de todas las experiencias/formatos con nombre propio |
| `10_SHOW_MUST_GO_ON.md` | Experiencia de vino, gastronomía y música en bodega centenaria |
| `11_SLOW_SESSIONS.md` | Formato boutique de naturaleza, enología y música acústica |
| `12_SIERRA_SALINAS.md` | Propuesta específica ligada a Slow Sessions |

### Temáticos

| Archivo | Contenido |
|---|---|
| `13_ARTISTAS_Y_BOOKING.md` | Programación artística — mayormente pendiente de definir |
| `14_SOSTENIBILIDAD.md` | Lo que el dossier dice sobre sostenibilidad — breve |
| `15_COMUNIDAD_DATOS_Y_ROI.md` | Comunidad, datos, retorno — mayormente pendiente de definir |
| `16_CASOS_DE_USO.md` | Escenarios hipotéticos de uso, explícitamente marcados como no confirmados |
| `17_BANCO_DE_IDEAS.md` | Ideas exploradas no confirmadas como oficiales — actualmente casi vacío |
| `19_ENTIDADES_RELACIONADAS.md` | Cómo distinguir Sabor a Música de ConcertSost y Fusion Town |

### Meta

| Archivo | Contenido |
|---|---|
| `18_PENDIENTES_Y_DECISIONES.md` | **Empezar por aquí si vas a ampliar esta base.** Lista completa de huecos, contradicciones y qué falta por confirmar |

## Qué archivos son más sólidos y cuáles son más débiles

**Sólidos** (basados en texto literal del dossier o en decisiones de diseño realmente tomadas y verificadas en la web publicada): `01`, `02` (parcial), `04`, `05` (parcial), `06` (parcial), `07`, `08`, `09`, `10`, `11`.

**Débiles / mayormente pendientes** (la plantilla pedía profundidad que no existe en las fuentes disponibles): `03` (parcial), `12`, `13`, `14`, `15`, `16` (hipotético por diseño), `17`.

## Cómo usar esta biblioteca en una conversación nueva

Sube toda la carpeta (o los archivos relevantes según la tarea) al inicio de la conversación. Para trabajo de contenido/tono, empieza por `01`, `02` y `07`. Para trabajo comercial, `03` y `06`. Para trabajo visual o de web, `08`. Para retomar o ampliar la base, `18` es obligatorio antes que nada.
