# Proyecto-CORTEX-Equipo-Visagismo

Este proyecto se basara en la programacion de un asistente, el cual tomara las medidas del rostro para calcular que corte de cabello sera el mas adecuado para el, este tomara en cuenta tambien el tipo de cabello, para un mejor resultado. Este metodo facilitara al cliente dejarse recomendar un corte de cabello, adecuado a su tipo de rostro.

## Fase 1 — Fundamentos del agente

### Semana 1 — Setup del entorno

El repositorio es público y cuenta con este `README.md`.

- **Nombre del equipo:** Proyecto-CORTEX-Equipo-Visagismo
- **Integrante:** Juan Navarro

### Semana 2 — Perfil del agente

#### 1. Perfil del Agente

<img width="1080" height="1350" alt="Digital Mind Map with Color-Coded Post-Its" src="https://github.com/user-attachments/assets/08a99a80-6b32-4fc0-ab61-8b794cd5dc49" />

<img width="1920" height="1080" alt="Infografía de tono de voz del barbero virtual" src="https://github.com/user-attachments/assets/772a85b8-caad-4d7c-b647-18627df1a8e1" />

### Semana 3 — Mapa de procesos cognitivos

<img width="800" height="2000" alt="Radar de procesos cognitivos del agente" src="https://github.com/user-attachments/assets/776d4f45-5c95-4d49-b58c-04c5f43c115f" />

La guía solicita Atención, Memoria, Lenguaje y Emoción. En la infografía se leen Atención 9, Lenguaje 8, Memoria 7 y Emoción 6, además de un quinto eje que también aparece como “Emoción” con puntuación 6. Se conserva la imagen original; el eje duplicado queda pendiente de aclaración.

## Fase 2 — Los sentidos del agente: inputs y filtros

### Semana 4 — Inventario de inputs: sensación y percepción

<img width="1024" height="768" alt="Mapa de inputs crudos y contexto del agente" src="https://github.com/user-attachments/assets/5893e32d-9d22-48a6-ba4e-178b62e6a434" />

### Semana 5 — Flujo perceptivo

Los diagramas disponibles describen el recorrido de los datos del cliente, la interpretación de rostro y cabello, las preferencias y la selección de opciones. La regla para distinguir una pregunta de una afirmación queda pendiente de acordar con el equipo.

<img width="3120" height="6404" alt="Flujo detallado de atención a una necesidad de cabello" src="https://github.com/user-attachments/assets/922bdfe6-f1c0-4d7b-8e21-be73aa518bdd" />

### Semana 6 — Filtro de atención

#### 2. Sistema de Percepción y Atención

REGLAS DE ATENCIÓN PARA ASISTENTE VIRTUAL DE VISAJISMO
##Reglas de atención del asistente
Este documento define el protocolo para procesar mensajes extensos y ofrecer respuestas precisas sobre visados. Aplica a todas las interacciones en las que el usuario envíe mensajes con más de 500 palabras.
Objetivo
Optimizar el tiempo de respuesta y la relevancia de la información entregada, enfocando el análisis en elementos clave y la solicitud concreta del usuario.
Protocolo de procesamiento de mensajes
1. Priorización de sustantivos clave
El asistente identificará y extraerá los sustantivos más relevantes relacionados con visajismo para orientar la respuesta:
Tipos de visa: turista, estudiante, trabajo, residencia.
País de destino y nacionalidad del solicitante.
Documentos: pasaporte, carta de invitación, reserva de vuelo, comprobantes financieros, seguros.
Plazos: fechas límite, tiempos de tramitación, vigencias.
Motivos de viaje: turismo, estudios, empleo, reagrupación familiar.
Situaciones especiales: menores de edad, antecedentes migratorios, rechazos previos, doble nacionalidad.
2. Análisis de la última frase
La frase final del mensaje tendrá prioridad, pues suele contener la pregunta o solicitud específica. Esta definirá el enfoque de la respuesta y los requisitos a destacar.
3. Descarte de información redundante
Se omitirá contexto excesivo, repeticiones y detalles no esenciales que no impacten directamente en:
Requisitos de visa.
Procedimientos y pasos de solicitud.
Documentación obligatoria y opcional.
Costos y plazos relevantes.
4. Respuesta enfocada
Con base en los sustantivos clave y la última frase, el asistente generará una respuesta:
Precisa, directa y accionable.
Limitada a la jurisdicción/consulado y tipo de visa mencionados.
Que liste documentos, pasos y plazos críticos, evitando información irrelevante del mensaje extenso.
Lineamientos de estilo de respuesta
Lenguaje claro y profesional.
Estructura por secciones o listas solo cuando aporten claridad.
Citas específicas a fuentes oficiales cuando se mencionen requisitos variables por país.
Solicitud de datos faltantes indispensables (p. ej., país de destino, nacionalidad, motivo del viaje).
Declaración final
Este mecanismo optimiza el tiempo de respuesta y mantiene la precisión en consultas complejas de visajismo.

## Fase 3 — Memoria y recuperación (Semanas 8–9)

### Semana 8 — La RAM cognitiva: memoria de trabajo y carga cognitiva

La consigna usa **7±2** como referencia didáctica. Para el proyecto se elige una ventana operativa de **7 mensajes recientes**. Cuando llega el octavo, se resume el contexto útil del mensaje más antiguo y se conserva un resumen breve junto a los siete mensajes recientes. El número describe esta política del bot; no es el límite técnico de tokens del modelo.

![Ventana de RAM con siete mensajes recientes y resumen del contexto anterior](docs/fase-3/diagramas/ventana-contexto.png)

[Documento de la Semana 8](docs/fase-3/semana-8-ventana-de-contexto.md) · [Fuente Mermaid editable](docs/fase-3/diagramas/ventana-contexto.mmd)

### Semana 9 — El Bibliotecario: procesos de recuperación y olvido

El flujo clasifica la pregunta, busca hasta cinco recuerdos del mismo usuario en LTM (similitud `> 0.70`), combina resultados pertinentes con el resumen y los siete mensajes recientes, responde y renueva el temporizador. Tras **10 minutos sin actividad**, cierra la sesión: guarda en LTM solo preferencias duraderas con consentimiento y vacía la RAM; sin consentimiento, solo la vacía. La retención LTM existente es de 90 días.

![Flujo de recuperación en LTM y cierre por diez minutos de inactividad](docs/fase-3/diagramas/recuperacion-olvido.png)

[Documento de la Semana 9](docs/fase-3/semana-9-recuperacion-y-olvido.md) · [Fuente Mermaid editable](docs/fase-3/diagramas/recuperacion-olvido.mmd)

#### Material visual adicional sin semana confirmada

<img width="2496" height="400" alt="Mi primer tablero (1)" src="https://github.com/user-attachments/assets/d47a61f3-b7fa-4b37-880d-ff8ce7e4f18b" />

#### Tablas e historial de memoria existentes

# 🗂️ Historial de recomendaciones

## 🧠 1. Memoria a Largo Plazo (LTM)

| Campo            | Tipo de dato | Descripción              | Ejemplo                  |
| ---------------- | ------------ | ------------------------ | ------------------------ |
| `id_memoria`     | INT          | Identificador de memoria | 001                      |
| `tipo_memoria`   | VARCHAR      | Tipo de memoria          | Semántica / Episódica    |
| `categoria`      | VARCHAR      | Categoría de información | Rostro / Cabello / Corte |
| `dato`           | TEXT         | Información almacenada   | Tipo de rostro: Ovalado  |
| `fecha_registro` | DATETIME     | Fecha de almacenamiento  | 2026-10-01               |

---

## 📚 2. Memoria Semántica

| Campo              | Tipo de dato | Descripción                | Ejemplo                                   |
| ------------------ | ------------ | -------------------------- | ----------------------------------------- |
| `id_semantica`     | INT          | Identificador              | 001                                       |
| `categoria`        | VARCHAR      | Categoría del conocimiento | Rostro                                    |
| `tipo_rostro`      | VARCHAR      | Forma del rostro           | Ovalado                                   |
| `tipo_cabello`     | VARCHAR      | Tipo de cabello            | Ondulado                                  |
| `textura`          | VARCHAR      | Textura del cabello        | Grueso                                    |
| `densidad`         | VARCHAR      | Densidad del cabello       | Media                                     |
| `nombre_corte`     | VARCHAR      | Corte registrado           | Taper Fade                                |
| `tipo_corte`       | VARCHAR      | Categoría del corte        | Taper                                     |
| `altura_degradado` | VARCHAR      | Altura del fade            | Bajo                                      |
| `volumen_superior` | VARCHAR      | Volumen del cabello        | Medio                                     |
| `compatibilidad`   | VARCHAR      | Compatibilidad con rostro  | Alta                                      |
| `codigo_intencion` | VARCHAR      | Intención reconocida       | `RECOMENDAR_CORTE`                        |
| `palabras_clave`   | TEXT         | Palabras asociadas         | "qué corte me queda", "qué corte me hago" |
| `regla_visajismo`  | TEXT         | Regla utilizada            | Mantener equilibrio visual del rostro     |

### Ejemplos de conocimiento semántico

| Tipo de rostro | Corte      | Compatibilidad | Regla                                 |
| -------------- | ---------- | -------------- | ------------------------------------- |
| Ovalado        | Taper Fade | Alta           | Mantiene proporciones equilibradas    |
| Ovalado        | Mid Fade   | Alta           | Permite diferentes estilos superiores |
| Redondo        | Taper Fade | Alta           | Favorece una apariencia más vertical  |
| Redondo        | Mid Fade   | Alta           | Reduce visualmente el volumen lateral |
| Cuadrado       | Mid Fade   | Alta           | Mantiene la estructura angular        |
| Alargado       | Low Fade   | Media          | Puede conservar mayor volumen lateral |
| Diamante       | Taper Fade | Alta           | Puede equilibrar los laterales        |
| Corazón        | Low Fade   | Media          | Ayuda a equilibrar frente y mandíbula |

---

## 🧠 3. Memoria Episódica

| Campo                 | Tipo de dato | Descripción                    | Ejemplo                          |
| --------------------- | ------------ | ------------------------------ | -------------------------------- |
| `id_episodio`         | INT          | Identificador del episodio     | 001                              |
| `id_usuario`          | INT          | Identificador del usuario      | 001                              |
| `consulta`            | TEXT         | Mensaje enviado por el usuario | "No sé qué corte me puedo hacer" |
| `intencion`           | VARCHAR      | Intención detectada            | `RECOMENDAR_CORTE`               |
| `tipo_rostro`         | VARCHAR      | Rostro identificado            | Ovalado                          |
| `tipo_cabello`        | VARCHAR      | Tipo de cabello                | Ondulado                         |
| `textura_cabello`     | VARCHAR      | Textura                        | Grueso                           |
| `densidad_cabello`    | VARCHAR      | Densidad                       | Media                            |
| `corte_recomendado`   | VARCHAR      | Corte recomendado              | Taper Fade                       |
| `cortes_alternativos` | TEXT         | Otras opciones                 | Mid Fade, Low Fade               |
| `preferencia_usuario` | TEXT         | Preferencia detectada          | Prefiere laterales cortos        |
| `fecha`               | DATETIME     | Fecha de interacción           | 2026-10-01                       |
## 🗂️ Carpetas de memoria del bot

| Carpeta de memoria                  | Información que debe conservar                               | Ejemplos                                                                                       |
| ----------------------------------- | ------------------------------------------------------------ | ---------------------------------------------------------------------------------------------- |
| 📐 **Tipos de rostro**              | Características y clasificación de las formas faciales       | Ovalado, redondo, cuadrado, rectangular, diamante, corazón, triangular                         |
| 💇 **Tipos de cabello**             | Características del cabello                                  | Liso, ondulado, rizado, afro                                                                   |
| 🧵 **Textura y densidad**           | Propiedades del cabello que afectan la elección del corte    | Fino, medio, grueso / baja, media, alta                                                        |
| ✂️ **Catálogo de cortes**           | Información sobre los cortes disponibles                     | Taper Fade, Low Fade, Mid Fade, High Fade, Mullet, Burst Fade, French Crop, Buzz Cut, Undercut |
| 📊 **Características de cortes**    | Propiedades de cada corte                                    | Altura del fade, volumen superior, volumen lateral, largo, mantenimiento                       |
| 🎨 **Reglas de visajismo**          | Reglas para relacionar rostro, cabello y corte               | Rostro redondo → controlar volumen lateral; rostro alargado → conservar equilibrio lateral     |
| 🔑 **Intenciones**                  | Acciones que puede solicitar el usuario                      | `RECOMENDAR_CORTE`, `ANALIZAR_ROSTRO`, `CONSULTAR_CORTE`, `COMPARAR_CORTES`                    |
| 🗣️ **Palabras clave**              | Palabras y frases utilizadas para identificar intenciones    | "qué corte me queda", "qué corte me hago", "tipo de rostro", "Taper Fade"                      |
| ⭐ **Compatibilidad**                | Relación entre tipos de rostro y cortes                      | Rostro ovalado + Taper Fade → compatibilidad alta                                              |
| 🧴 **Cuidado y mantenimiento**      | Información sobre mantenimiento de cada estilo               | Frecuencia de corte, productos, peinado                                                        |
| 👤 **Preferencias del usuario**     | Preferencias que pueden personalizar futuras recomendaciones | Prefiere laterales cortos, no quiere mucho volumen, prefiere estilos modernos                  |
| 💬 **Historial de recomendaciones** | Recomendaciones realizadas anteriormente                     | Corte recomendado, alternativas y motivo de la recomendación                                   |

#### Diseño propuesto que sustituye al código anterior

El bloque de Python anterior no era el entregable solicitado. Se reemplaza por la definición visual y lógica de la memoria de trabajo y del flujo de recuperación; esta sección describe el diseño, no afirma que haya un backend desplegado.

| Parte | Regla definida para el bot |
| --- | --- |
| Ventana RAM | Mantener los 7 mensajes recientes; el número 7±2 sirve como referencia didáctica, no como límite del modelo. |
| Desborde | Al llegar un nuevo mensaje que exceda la ventana, resumir el mensaje más antiguo y conservar el resumen con los 7 mensajes recientes. |
| Recuperación LTM | Clasificar tema/intención, buscar por usuario y tema, usar hasta 5 recuerdos con similitud > 0.70 y combinarlos con el contexto reciente. |
| Olvido | Tras 10 minutos sin actividad, vaciar la RAM. Guardar preferencias duraderas en LTM solo con consentimiento; retención propuesta: 90 días. |

Los diagramas están arriba, en las secciones de Semana 8 y Semana 9. Consulta las [reglas de RAM de la Semana 8](docs/fase-3/semana-8-ventana-de-contexto.md) y el [flujo del Bibliotecario de la Semana 9](docs/fase-3/semana-9-recuperacion-y-olvido.md). El código original se conserva en [`docs/README-original.md`](docs/README-original.md), no como la solución activa.

## Material complementario — Fase y semana por confirmar

Estos materiales siguen visibles y conservados; aún no se han asignado a una semana de las guías recibidas:

`  ![Uploading flujo-sarcasmo.png…]()`

`![Uploading diagrama.svg…]()`

También se conservan los diagramas complementarios existentes:

<img width="1920" height="1080" alt="Diagrama de manejo de ambigüedad, caso borde" src="https://github.com/user-attachments/assets/3dc15455-8f26-4c89-8139-f9177fa352f8" />

<img width="1920" height="1080" alt="Simulación de diálogo Golden Samples" src="https://github.com/user-attachments/assets/6fd8818c-8e51-4c58-8aa3-4ea9d56ed6f6" />

<img width="808" height="1236" alt="Flujo de captura de datos y recomendación de estilo" src="https://github.com/user-attachments/assets/f4345a55-1347-4a8c-89f9-8b4eed275eb0" />

### Seguridad y ética

# Seguridad y ética del asistente de visagismo

## Bug humano identificado: sesgo de género

El asistente podría heredar un sesgo de género si relaciona ciertos cortes o peinados exclusivamente con hombres o con mujeres, o si recomienda un estilo según el género que cree que tiene el cliente. Esto podría limitar las opciones ofrecidas y hacer que la recomendación no refleje lo que la persona realmente desea.

## Regla de seguridad

1. No infieras el género, la identidad de género ni la expresión de género de una persona a partir de su nombre, apariencia, fotografía u otros datos indirectos.
2. No presentes ningún corte, peinado o estilo como exclusivo o adecuado únicamente para hombres o para mujeres.
3. Basa las recomendaciones en las preferencias expresadas por el cliente: el estilo que busca, el largo que prefiere, el mantenimiento que acepta y el resultado que desea.
4. Ten en cuenta solo la información relevante sobre el cabello y el rostro que el cliente haya indicado o que se observe claramente. No inventes características ni las deduzcas a partir del género.
5. Si falta información necesaria para recomendar, haz una pregunta neutral antes de responder.
6. Ofrece opciones variadas y descríbelas sin juzgar ni imponer una expresión de género.
7. Si el cliente pide expresamente una estética masculina, femenina o andrógina, puedes usar esa preferencia para orientar las opciones, sin asumir que define su identidad.

## Lógica y ética

La recomendación debe basarse en las preferencias del cliente y en los datos relevantes sobre su cabello y rostro, no en suposiciones sobre su género. Así se evita que un estereotipo reduzca las opciones disponibles. Éticamente, la regla promueve un trato respetuoso y equitativo: cada persona recibe recomendaciones acordes con lo que busca, sin ser juzgada ni encasillada. Si falta información, el asistente debe preguntar en lugar de adivinar.

La copia íntegra del README anterior permanece en [`docs/README-original.md`](docs/README-original.md). Los documentos detallados están en `docs/fase-1/`, `docs/fase-2/` y [`docs/fase-3/`](docs/fase-3/README.md); el resumen por fases está en [`docs/organizacion-por-fases.md`](docs/organizacion-por-fases.md).
