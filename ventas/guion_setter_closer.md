# FinanzasconNico — Guion de setter (bot) y closer

Objetivo: que cada persona que escribe una palabra clave de un Reel (REVISIÓN, HERENCIA, CAMPO, NVIDIA, TRAER…) termine en una **llamada de 15 minutos con Nico** y, de ahí, en una **cuenta abierta**.

Embudo: Reel → mensaje con palabra clave → **setter (bot)** califica y agenda → **closer (Nico)** cierra en la llamada → seguimiento.

---

## Reglas para todo el embudo (no negociables)

- El bot **se presenta como asistente automático** de Nico. Nunca se hace pasar por él.
- El bot **no da recomendaciones de inversión, no promete rendimientos ni habla de "ganancias seguras"**. Solo informa, hace preguntas y agenda.
- Toda propuesta concreta la hace Nico, **después del perfil de inversor**, y siempre con la aclaración de que los rendimientos no están garantizados.
- Datos sensibles (DNI, montos exactos, extractos) **no se piden por el bot**: se ven en la llamada o por los canales de Balanz.
- Si la persona pide hablar con un humano, está enojada o pregunta algo fuera del guion → **pasa a Nico de inmediato**.

---

## PARTE 1 — Setter (lo que hace el bot)

### Paso 1 · Respuesta inmediata (en menos de 1 minuto)
> ¡Hola {nombre}! 👋 Soy el asistente de Nico (FinanzasconNico). Vi que escribiste **{PALABRA}**. Te hago 3 preguntas rápidas así Nico llega a la charla con tu caso ya entendido, ¿dale?

### Paso 2 · Calificación (una pregunta por mensaje)
1. **Situación** (según la palabra clave):
   - REVISIÓN → "¿Hoy tenés inversiones? ¿Dónde: banco, broker, plazo fijo, dólares guardados?"
   - HERENCIA → "¿Ya tenés acceso a la cuenta o todavía está en trámite la sucesión?"
   - CAMPO → "¿Cuándo te entra la plata de la cosecha, más o menos?"
   - TRAER → "¿Tenés los dólares en una cuenta afuera a tu nombre?"
   - NVIDIA / noticias → "¿Ya tenés esa acción o estás pensando en entrar?"
2. **Rango de capital** (con opciones, sin pedir número exacto):
   > "Para orientar a Nico, ¿en qué rango estás? a) menos de USD 5.000 · b) 5.000–30.000 · c) 30.000–100.000 · d) más de 100.000"
3. **Urgencia**:
   > "¿Esto lo querés resolver ahora o es para más adelante?"

### Paso 3 · Agendar
- **Calificado** (b, c o d, o urgencia alta):
  > "Perfecto. Lo mejor es una llamada de 15 minutos con Nico, sin costo y sin compromiso. Tengo {día} a las {hora} o {día} a las {hora}, ¿cuál te queda mejor?"
  → Confirmar, mandar recordatorio el día anterior y 1 hora antes.
- **No calificado todavía** (a, o "más adelante"):
  > "¡Genial! Te dejo esta guía para arrancar: https://finanzasconnico-web.vercel.app/guia.html. Cuando quieras dar el paso, escribime de nuevo y lo vemos."
  → Etiquetar como "nutrir" y reenviarle contenido útil cada 2–3 semanas.

### Paso 4 · Pasar la ficha a Nico
Antes de la llamada, el bot le manda a Nico un resumen:
`Nombre · Palabra clave · Situación · Rango · Urgencia · Día y hora`

---

## PARTE 2 — Closer (la llamada de 15 minutos de Nico)

### 1. Apertura (1 min) — marco y permiso
> "Gracias por agendar, {nombre}. La idea es: entender tu situación, decirte con honestidad si te puedo ayudar, y si tiene sentido, contarte cómo trabajaríamos. Si no te sirvo, te lo digo. ¿Te parece?"

### 2. Diagnóstico (5–6 min) — que hable el cliente
- "Contame qué tenés hoy y dónde."
- "¿Qué te hizo escribirme justo ahora?" ← **el motivo real de compra**
- "¿Qué te preocupa más: perder contra la inflación, el dólar, no entender lo que tenés, otra cosa?"
- "Si dentro de un año esto está resuelto, ¿cómo se ve?"
- "¿Alguien más decide esto con vos?" (pareja, socio, hermanos)
- **Perfil**: horizonte de tiempo, cuánto necesita tener disponible, cómo reacciona si algo baja un 10%.

Regla: **80% habla el cliente, 20% Nico.** Anotar sus palabras textuales para usarlas después.

### 3. Resumen (1 min) — "¿entendí bien?"
> "Entonces, si te entendí bien: tenés {X} en {dónde}, te preocupa {Y} y querés {Z}. ¿Es así?"

### 4. Propuesta (3 min) — usando SUS palabras
- Explicar en 3 puntos simples cómo lo resolverían (sin jerga).
- Costos claros: "No te cobro por asesorarte; hay una comisión por operación que sabés antes de hacerla."
- Seguridad: "La cuenta está a tu nombre en Balanz, regulada por la CNV. Yo no toco tu plata sin tu aprobación."
- Siempre: "Los rendimientos no están garantizados; lo que sí te garantizo es que vas a entender todo lo que hacemos."

### 5. Cierre (2 min) — pregunta directa
> "¿Te parece que abramos la cuenta ahora así lo dejamos andando? Son 10 minutos y lo hacemos juntos."

Si duda → **silencio**. Dejar que hable primero.

### 6. Objeciones frecuentes
| Objeción | Respuesta |
|---|---|
| "Lo tengo que pensar" | "Totalmente. ¿Qué parte te gustaría pensar? Así te paso lo que necesites para decidir." |
| "Ya tengo banco / otro asesor" | "Bien. ¿Sabés cuánto te rinde y cuánto te cobran? Si querés lo comparamos con números y decidís vos." |
| "No confío en dejar la plata" | "Es lógico. La cuenta es tuya, a tu nombre, en Balanz regulada por la CNV. Podés ver y retirar cuando quieras." |
| "Es poca plata" | "Se puede empezar con poco. Lo importante es el hábito y que entiendas qué hacés." |
| "Ahora con el dólar así, mejor espero" | "Justamente en momentos así conviene tener un plan. No hace falta mover todo; podemos empezar con una parte." |
| "Lo consulto con mi pareja / socio" | "Perfecto, ¿agendamos 15 minutos los tres así le explico directo?" |

### 7. Seguimiento si no cerró
- Mismo día: resumen por escrito de lo hablado + próximo paso.
- Día 3: algo útil (un video o dato relacionado con su caso), sin presión.
- Día 7: "¿Pudiste pensarlo? ¿Lo dejamos andando esta semana?"
- Después: pasa a "nutrir" (contenido cada 2–3 semanas).

---

## Métricas a mirar cada semana
- Mensajes con palabra clave (por Reel)
- % que responde las 3 preguntas del bot
- % que agenda
- % que asiste a la llamada
- % que abre cuenta (**cierre**)
