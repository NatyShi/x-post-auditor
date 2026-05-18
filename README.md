# X Post Auditor - Optimizá tus posts para el algoritmo de X

**Herramienta gratuita para analizar y mejorar tus posts antes de publicarlos**, basada en el código oficial del algoritmo de X publicado por xAI en GitHub.

→ **[Usá la herramienta ahora](https://TU-USUARIO.github.io/x-post-auditor/)** *(reemplazá con tu URL de GitHub Pages)*

Creada por **[@NatyShi_](https://x.com/NatyShi_)** - solopreneur, product builder.

---

## ¿Qué hace?

Pegás el texto de tu próximo post, marcás qué tipo de contenido es y qué incluye, y la herramienta te devuelve:

- **Score de 0 a 100** según las señales que pondera el algoritmo real de X
- **Señales detectadas** - qué está sumando y qué está restando puntos, con explicación de por qué
- **Recomendaciones accionables** - cambios concretos para mejorar el post antes de publicar
- **Previsualización en tiempo real** - ves exactamente cómo se ve el post en el feed, dónde corta con "Mostrar más" y en qué zona de longitud estás (óptima / larga / truncada)

Todo corre en tu navegador. No hay servidor, no se envían datos a ningún lado.

---

## ¿Por qué esto importa?

El algoritmo de X no distribuye todos los posts por igual. Prioriza contenido que genera **replies, dwell time y compartidos**, y penaliza links externos en el cuerpo, exceso de hashtags y patrones de engagement bait.

Sin conocer esas reglas, podés estar publicando contenido que el propio algoritmo suprime antes de que llegue a tu audiencia.

---

## Señales que analiza

| Señal | Lógica del algoritmo |
|---|---|
| **Link en el cuerpo** | Penalización del 30-50% de alcance - X retiene al usuario en la plataforma |
| **Replies / CTA** | La señal de mayor peso. Más que likes o retweets |
| **Video** | Activa el scorer VQV (video quality view) - dwell time máximo |
| **Imagen** | Dispara la señal `photo_expand` |
| **Poll** | Genera dwell time + click obligatorio para votar |
| **Hashtags** | El algoritmo 2025-2026 usa embeddings semánticos, no hashtags |
| **Longitud** | 60-280 chars = zona óptima. Más de 280 = truncado con "Mostrar más" |
| **Tipo de post** | RT puro / RT con cita / reply / hilo tienen pesos distintos |

---

## Tipos de contenido soportados

- ✏️ Post original
- 💬 RT con cita
- ↩️ Reply a otro post
- 🧵 Hilo (primer tweet)
- 🔁 RT sin texto

---

## Cómo usarla

**Opción A - Online (recomendado):**
Entrá al link de GitHub Pages de arriba. Funciona directo en el navegador.

**Opción B — Local:**
1. Descargá el archivo `auditor_x.html`
2. Abrilo con doble click en cualquier navegador
3. No necesita instalación ni conexión a internet (salvo la tipografía de Google Fonts)

---

## Stack

HTML + CSS + JavaScript vanilla. Sin dependencias, sin frameworks, sin backend.
Un solo archivo autocontenido.

---

## Fork / Contribuciones

Podés forkear este repo y adaptarlo a tu caso. Ideas para extender:

- Soporte para otros idiomas
- Integración con la API de X para analizar posts ya publicados
- Historial de posts analizados (localStorage)
- Modo comparación A/B entre dos versiones del mismo post

Si lo usás o lo adaptás, un mention a [@NatyShi_](https://x.com/NatyShi_) es siempre bienvenido. 🙌

---

## Fuente del algoritmo

Basado en el código publicado por xAI en [github.com/xai-org/x-algorithm](https://github.com/xai-org/x-algorithm).
Los pesos y señales reflejan el comportamiento documentado al momento de construcción de esta herramienta (mayo 2026).

---

*Construido con obsesión por el producto y sin presupuesto de ads. Así se hace.*
