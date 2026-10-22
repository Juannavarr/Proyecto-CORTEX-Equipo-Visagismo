<img width="1024" height="768" alt="Colorful Simple Creative Modern Mind Map Graph" src="https://github.com/user-attachments/assets/5893e32d-9d22-48a6-ba4e-178b62e6a434" />
# Proyecto-CORTEX-Equipo-Visagismo
Este proyecto se basara en la programacion de un asistente, el cual tomara las medidas del rostro para calcular que corte de cabello sera el mas adecuado para el, este tomara en cuenta tambien el tipo de cabello, para un mejor resultado. Este metodo facilitara al cliente dejarse recomendar un corte de cabello, adecuado a su tipo de rostro.
##1.Perfil del Agente.
<img width="1080" height="1350" alt="Digital Mind Map with Color-Coded Post-Its" src="https://github.com/user-attachments/assets/08a99a80-6b32-4fc0-ab61-8b794cd5dc49" />
<img width="800" height="2000" alt="Infografía profesional con gráfico de radar" src="https://github.com/user-attachments/assets/776d4f45-5c95-4d49-b58c-04c5f43c115f" />
<img width="2496" height="400" alt="Mi primer tablero (1)" src="https://github.com/user-attachments/assets/d47a61f3-b7fa-4b37-880d-ff8ce7e4f18b" />
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
"""
Asistente de visajismo - Memoria LTM + RAM + Regla de Olvido
Pegar completo en un archivo: bot.py
"""

import os
import json
from datetime import datetime, timedelta

import redis
import psycopg2
from psycopg2.extras import RealDictCursor
from openai import OpenAI

# ─────────── CONFIG ───────────
REDIS_URL = os.getenv("REDIS_URL", "redis://localhost:6379/0")
POSTGRES_URL = os.getenv("POSTGRES_URL", "postgresql://user:pass@localhost/visas")
OPENAI_API_KEY = os.getenv("OPENAI_API_KEY")

RAM_TTL_SECONDS = 600      # 10 min inactividad → borra RAM
MAX_TURNOS_RAM = 30        # comprime si supera 30 turnos
DIAS_RETENCION_LTM = 90    # purga LTM a los 90 días
TOP_K_LTM = 5

redis_client = redis.from_url(REDIS_URL, decode_responses=True)
client = OpenAI(api_key=OPENAI_API_KEY)


# ─────────── RAM ───────────
def _ram_key(user_id, session_id):
    return f"ram:{user_id}:{session_id}"


def get_ram(user_id, session_id):
    data = redis_client.get(_ram_key(user_id, session_id))
    return json.loads(data) if data else []


def save_ram(user_id, session_id, turnos):
    if len(turnos) > MAX_TURNOS_RAM:
        antiguos = turnos[:-10]
        resumen = "[RESUMEN PREVIO] " + " | ".join(
            f"{t['role']}: {t['content'][:80]}" for t in antiguos
        )
        turnos = [{"role": "system", "content": resumen}] + turnos[-10:]
    # TTL: la regla de olvido se aplica sola aquí
    redis_client.setex(_ram_key(user_id, session_id),
                       RAM_TTL_SECONDS,
                       json.dumps(turnos, ensure_ascii=False))


def clear_ram(user_id, session_id):
    redis_client.delete(_ram_key(user_id, session_id))


# ─────────── LTM ───────────
def _conn():
    return psycopg2.connect(POSTGRES_URL, cursor_factory=RealDictCursor)


def embed(texto):
    r = client.embeddings.create(model="text-embedding-3-small", input=texto)
    return r.data[0].embedding


def buscar_ltm(user_id, embedding, tema=None):
    conn = _conn()
    cur = conn.cursor()
    if tema:
        cur.execute("""
            SELECT contenido, fuente, 1 - (embedding <=> %s::vector) AS sim
            FROM ltm_usuario
            WHERE user_id = %s AND (tema = %s OR tema IS NULL)
            ORDER BY embedding <=> %s::vector LIMIT %s
        """, (embedding, user_id, tema, embedding, TOP_K_LTM))
    else:
        cur.execute("""
            SELECT contenido, fuente, 1 - (embedding <=> %s::vector) AS sim
            FROM ltm_usuario
            WHERE user_id = %s
            ORDER BY embedding <=> %s::vector LIMIT %s
        """, (embedding, user_id, embedding, TOP_K_LTM))
    rows = cur.fetchall()
    cur.close(); conn.close()
    return [r for r in rows if r["sim"] > 0.7]


def guardar_ltm(user_id, contenido, embedding, tema=None,
                tipo="dato", fuente=None):
    conn = _conn()
    cur = conn.cursor()
    cur.execute("""
        INSERT INTO ltm_usuario
        (user_id, contenido, embedding, tema, tipo, fuente, fecha_actualizacion)
        VALUES (%s, %s, %s, %s, %s, %s, NOW())
    """, (user_id, contenido, embedding, tema, tipo, fuente))
    conn.commit(); cur.close(); conn.close()


# ─────────── REGLA DE OLVIDO ───────────
def al_expirar_sesion(user_id, session_id):
    """Antes de que Redis borre la RAM, rescata lo importante a LTM."""
    turnos = get_ram(user_id, session_id)
    if not turnos:
        return
    texto = "\n".join(f"{t['role']}: {t['content']}" for t in turnos)
    r = client.chat.completions.create(
        model="gpt-4o-mini",
        messages=[
            {"role": "system", "content": "Extrae SOLO: datos personales, "
             "casos pendientes, preferencias. Máximo 3 líneas."},
            {"role": "user", "content": texto}
        ]
    )
    resumen = r.choices[0].message.content
    guardar_ltm(user_id, resumen, embed(resumen), tipo="resumen_sesion")


def purgar_ltm_antigua():
    """Job diario: borra LTM con más de DIAS_RETENCION_LTM días."""
    conn = _conn(); cur = conn.cursor()
    cur.execute("DELETE FROM ltm_usuario WHERE fecha_actualizacion < %s",
                (datetime.now() - timedelta(days=DIAS_RETENCION_LTM),))
    conn.commit(); cur.close(); conn.close()


# ─────────── FASE 2 + FASE 3 ───────────
def clasificar(pregunta):
    r = client.chat.completions.create(
        model="gpt-4o-mini",
        response_format={"type": "json_object"},
        messages=[
            {"role": "system", "content": 'Devuelve JSON: '
             '{"intencion": "...", "entidad": "...", "tema": "..."}'},
            {"role": "user", "content": pregunta}
        ]
    )
    return json.loads(r.choices[0].message.content)


def responder(pregunta, user_id, session_id):
    # 1. RAM actual
    ram = get_ram(user_id, session_id)

    # 2. FASE 2: clasificar
    meta = clasificar(pregunta)
    tema = meta.get("tema")

    # 3. FASE 3: buscar en LTM
    emb = embed(pregunta)
    docs = buscar_ltm(user_id, emb, tema=tema)
    ctx = "\n".join(f"- {d['contenido']}" for d in docs) \
        if docs else "Sin info previa del usuario."

    # 4. Construir prompt
    mensajes = [
        {"role": "system", "content": "Eres un asistente experto en visajismo."},
        {"role": "system", "content": f"[CONTEXTO LTM]\n{ctx}"},
    ] + ram + [{"role": "user", "content": pregunta}]

    # 5. Responder
    r = client.chat.completions.create(model="gpt-4o-mini", messages=mensajes)
    respuesta = r.choices[0].message.content

    # 6. Actualizar RAM (TTL se renueva)
    ram.append({"role": "user", "content": pregunta})
    ram.append({"role": "assistant", "content": respuesta})
    save_ram(user_id, session_id, ram)

    return respuesta


# ─────────── USO ───────────
if __name__ == "__main__":
    r = responder(
        pregunta="¿Necesito cita para visa Canadá?",
        user_id="573001234567",
        session_id="573001234567_1730000000"
    )
    print(r)
  ![Uploading flujo-sarcasmo.png…]()
<img width="1920" height="1080" alt="Diagrama de detección de sarcasmo" src="https://github.com/user-attachments/assets/772a85b8-caad-4d7c-b647-18627df1a8e1" />
<img width="1920" height="1080" alt="Diagrama de detección de sarcasmo (3)" src="https://github.com/user-attachments/assets/3dc15455-8f26-4c89-8139-f9177fa352f8" />
<img width="1920" height="1080" alt="Diagrama de detección de sarcasmo (1)" src="https://github.com/user-attachments/assets/6fd8818c-8e51-4c58-8aa3-4ea9d56ed6f6" />
<img width="3120" height="6404" alt="image" src="https://github.com/user-attachments/assets/922bdfe6-f1c0-4d7b-8e21-be73aa518bdd" />
