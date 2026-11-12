# Fase 2 — Semana 4: Inventario de inputs

La actividad distingue **sensación** (datos que entran) de **percepción** (interpretación básica que hace el agente). El material visual de Miro agrupa la entrada visual, rasgos del rostro y cabello, señales del mensaje y contexto.

![Mapa de inputs crudos y contexto del agente](https://github.com/user-attachments/assets/5893e32d-9d22-48a6-ba4e-178b62e6a434)

## Clasificación de los inputs

| Input crudo (sensación) | Interpretación básica (percepción) | Uso previsto |
|---|---|---|
| Foto frontal o de perfil aportada por el cliente | Rasgos y proporciones visibles del rostro | Orientar opciones de estilo; no inferir características que no se distingan claramente. |
| Descripción del cabello o imagen del cabello | Tipo, textura, densidad, grosor y patrones de crecimiento que se puedan identificar | Considerar la viabilidad y el mantenimiento del corte. Si falta un dato, preguntar. |
| Texto escrito por el cliente | Solicitud, preferencias, límites y datos que comunica explícitamente | Entender qué cambio busca antes de recomendar. |
| Emojis, longitud del mensaje, formalidad y jerga | Señales contextuales posibles sobre tono o urgencia | Usarlas con cautela; no diagnosticar ni asumir un estado emocional a partir de una sola señal. |
| Nota de voz, si el usuario la envía | Contenido hablado y rasgos audibles del mensaje | Considerarla solo si la aplicación procesa audio y esa señal es pertinente. |
| Hora, dispositivo o ubicación, si están disponibles y son pertinentes | Contexto de la interacción | No tratar metadatos como obligatorios ni deducir información personal innecesaria. |

## Elementos que no son sensores

En la lámina, algunas zonas describen el **rol del bot** y su **tono de voz**. Son parte del perfil del agente, no inputs del cliente; por eso se documentan en [Semana 2 — Perfil del agente](../fase-1/semana-2-perfil-del-agente.md).
