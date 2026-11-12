# Organización del proyecto por fases

Este documento reúne en un solo lugar las fases que ya se pudieron organizar y el material que sigue pendiente de ubicar. El alcance actual llega hasta la **Fase 2 (Semana 6)**. Las fases posteriores no se asignan por suposición: se ordenarán cuando se compartan sus guías. El contenido fuente permanece conservado en [`README-original.md`](README-original.md).

## Fase 1 — Fundamentos del agente (Semanas 1–3)

### Semana 1 — Setup del entorno

**Entregable solicitado:** repositorio público con `README.md`, nombre del equipo e integrantes.

**Estado:** repositorio público con README. Equipo: **Proyecto-CORTEX-Equipo-Visagismo**. Integrante registrado: **Juan Navarro**.

### Semana 2 — Perfil y personalidad del agente

**Entregable solicitado:** definir en Miro quién es el bot, a quién ayuda, su tono y su rol psicológico; transferir el resumen a GitHub bajo `## 1. Perfil del Agente`.

**Resumen organizado:** el agente es un asesor de imagen digital basado en visagismo para barbería. Ayuda a clientes a explorar cortes y estilos de barba considerando sus rasgos, cabello y preferencias. Su tono es cercano, conversacional, cálido y honesto. Orienta sin juzgar ni imponer; la decisión final corresponde al cliente.

**Material existente:** mapa de perfil y lámina de tono de voz, enlazados en el README del repositorio y conservados en el archivo original.

### Semana 3 — Mapa de procesos cognitivos

**Entregable solicitado:** gráfico de radar con puntuaciones de Atención, Memoria, Lenguaje y Emoción (1–10) y una justificación teórica breve.

**Valores legibles en la imagen existente:** Atención 9/10; Lenguaje 8/10; Memoria 7/10; Emoción 6/10. La imagen además presenta un quinto eje con la etiqueta “Emoción” y puntuación 6. Se conserva sin cambios; el significado del eje duplicado queda pendiente de confirmar con el equipo.

## Fase 2 — Los sentidos del agente: inputs y filtros (Semanas 4–6)

### Semana 4 — Inventario de inputs: sensación y percepción

**Entregable solicitado:** inventariar en Miro qué entradas recibe el bot y clasificarlas como datos crudos (sensación) o interpretaciones básicas (percepción); subir una captura a GitHub.

**Resumen organizado:** entre los inputs crudos del material están las fotos o descripciones del rostro y el cabello, los mensajes de texto y, si se usan, las notas de voz y señales de contexto. Entre las interpretaciones aparecen la forma y proporciones faciales, características del cabello e intención del mensaje. El rol y el tono del bot pertenecen a su perfil, no son inputs del usuario.

**Material existente:** mapa visual de inputs crudos y contexto, vinculado desde el README.

### Semana 5 — Flujo perceptivo

**Entregable solicitado:** dibujar el recorrido del dato desde que entra hasta que se considera útil y definir una regla sencilla para distinguir una pregunta de una afirmación.

**Resumen organizado:** los diagramas disponibles recorren la recopilación de datos del cliente, la identificación de información faltante, la confirmación de preferencias y límites, la selección de opciones compatibles y la presentación de una recomendación que puede ajustarse según la respuesta del cliente.

**Pendiente de completar:** no se encontró una regla explícita y acordada para distinguir preguntas de afirmaciones. Debe definirse con el equipo; no se inventa aquí.

### Semana 6 — Filtro de atención

**Entregable solicitado:** explicar en GitHub qué se considera ruido y documentar las reglas de atención selectiva.

**Resumen organizado del material existente:** para mensajes de más de 500 palabras, priorizar sustantivos clave y la última frase, descartar repeticiones y pedir datos indispensables que falten.

**Pendiente de aclaración:** el bloque original incluye términos sobre visas, consulados y países, aunque su título lo presenta como una regla para el asistente de visagismo. Esas referencias se preservan sin reinterpretación hasta conocer el contexto de las otras fases.

## Fase 3 — Memoria y recuperación (Semanas 8–9)

### Semana 8 — La RAM cognitiva

Se usa **7±2** como referencia didáctica y se fija una ventana de **7 mensajes recientes**. Al llegar un nuevo mensaje que supera el límite, se comprime lo más antiguo en un resumen y se conservan los siete más recientes. El límite de siete es una regla de diseño, no el límite técnico de tokens del modelo. [Documento y diagrama](fase-3/semana-8-ventana-de-contexto.md).

### Semana 9 — El Bibliotecario

El prototipo ya tiene búsqueda LTM por usuario/tema, `TOP_K_LTM = 5`, similitud `> 0.70`, retención de 90 días y expiración RAM de 10 minutos. La política define cómo combinar recuerdos y contexto actual, y borrar RAM tras la inactividad. Falta conectar el finalizador a un temporizador real antes de que expire la clave Redis. [Documento y diagrama](fase-3/semana-9-recuperacion-y-olvido.md).

## Material que todavía no se ha podido asignar a una fase

Las guías recibidas llegan hasta la Semana 9. Estos otros elementos se conservan como **pendientes de clasificar**, sin adjudicarles una semana:

- Diagramas complementarios de sarcasmo, manejo de ambigüedad y ejemplos de diálogo.
- Material sobre sesgo de género, seguridad y ética, junto con su diagrama.
- Diagrama horizontal panorámico cuyo título no permite identificar con seguridad su semana.
- Referencias a visas y consulados hasta confirmar a qué actividad pertenecen.

Este material **no se elimina**. Se mantiene completo en [`README-original.md`](README-original.md) y está listado también en [`pendiente-de-clasificar.md`](pendiente-de-clasificar.md). Cuando se compartan las próximas guías, se podrá colocar cada elemento en su fase y semana correctas.
