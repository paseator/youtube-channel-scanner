# YouTube Channel Scanner

Pega en un asistente de IA la lista de tus Shorts y Vídeos de YouTube Studio y obtén un informe de una página que muestra qué has publicado y dónde se acumulan tus vistas.

Versión 1.0.0. Versión en español. [English version](README.md)

## Qué hace

El prompt convierte tu propia lista de YouTube Studio en un único informe HTML en A4 con:

- Publicaciones analizadas, vistas totales y cantidad de Shorts y Vídeos.
- Hasta cinco grupos de contenido, más una fila «Otros», propuestos a partir de tus títulos y descripciones, cada uno con su porcentaje de vistas.
- Un gráfico circular de vistas por formato.
- La audiencia y la temática a las que parecen dirigirse tus publicaciones, y hasta cuatro necesidades que abordan.
- Un hallazgo y una prueba posible.
- Notas sobre lo que los datos no pueden mostrar.

El informe se escribe en español y termina con un pie breve con la web, una línea de crédito y la fecha de generación.

## Qué no hace

Describe lo que ya has publicado. No investiga el mercado, tu audiencia real ni tu competencia, y no explica por qué un canal crece o se estanca, ni valida un nicho, ni promete crecimiento o monetización.

## Cómo se usa

1. Abre `youtube-channel-scanner-prompt-ES.txt` y pega todo su contenido en un asistente de IA.
2. El asistente responde con instrucciones. En YouTube Studio, entra en **Contenido**, elige la pestaña **Shorts** y/o **Vídeos**, selecciona la tabla desde la cabecera hasta la última fila y cópiala.
3. Pega la lista en el chat. Puedes enviarla en varios bloques. Tras cada uno, el asistente confirma cuántas publicaciones válidas y únicas lleva.
4. Cuando no tengas nada más que añadir, responde **No**. El asistente genera entonces el informe.

El informe es un archivo HTML llamado `informe-parasite.html`. Funciona sin conexión y está pensado para imprimirse en una página A4. El asistente debe poder crear o exportar archivos; si no puede, el prompt le indica que lo diga en lugar de simular la entrega.

## Cómo se trata tu lista

- Cada publicación necesita al menos un título y las vistas. La fecha, la descripción, la duración y los comentarios son opcionales. Lo que falta se marca como no disponible y nunca se cuenta como cero. Un cero que hayas pegado se conserva como cero.
- El formato (Short o Vídeo) se toma de la pestaña o de la cabecera de cada bloque que pegues, no de la duración ni del título. Si un bloque no se puede identificar, sus publicaciones aparecen como «Sin identificar».
- Los duplicados se detectan y se cuentan una sola vez.
- Los títulos y descripciones pegados se tratan como datos a analizar, no como instrucciones.
- Solo se analiza la lista que compartes. Las fechas de publicación no son las fechas en que se obtuvieron las vistas, y las vistas no muestran retención, satisfacción ni comunidad.

## Privacidad

Este repositorio solo contiene archivos de texto y no recoge nada. La lista que pegas la procesa el asistente de IA que elijas, bajo las condiciones de ese servicio, así que revísalas si tus datos son sensibles. El prompt indica al asistente que use solo lo que pegues, sin búsquedas web, APIs ni conexiones a cuentas.

## Archivos

- `youtube-channel-scanner-prompt-EN.txt`: prompt en inglés.
- `youtube-channel-scanner-prompt-ES.txt`: prompt en español.
- `LICENSE`: texto legal de CC BY 4.0.
- `NOTICE`: copyright, crédito y lo que la licencia no cubre.

## Licencia

[Creative Commons Atribución 4.0 Internacional (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/deed.es). Puedes usarlo, modificarlo y compartirlo, incluso comercialmente, si reconoces al autor, enlazas la licencia e indicas los cambios. Se ofrece sin garantías.

Crédito sugerido:

> Basado en YouTube Channel Scanner de Paul Ramirez, PARASITE INTELLIGENCE (https://www.parasiteintelligence.com), CC BY 4.0.

La licencia no hace públicas tus propias listas ni tus informes.

## Autor

Paul Ramirez, [parasiteintelligence.com](https://www.parasiteintelligence.com)
