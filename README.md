# X Post Auditor - Optimizá tus posts para el algoritmo 2026 de X | Optimize your posts for the 2026 X algorithm

| Español | English |
|---|---|
| **Herramienta gratuita para analizar y mejorar tus posts antes de publicarlos**, basada en el código oficial del algoritmo de X publicado por xAI en GitHub. | **Free tool to analyze and improve your posts before publishing them**, based on the official X algorithm code published by xAI on GitHub. |
| → **[Usá la herramienta ahora](https://natyshi.github.io/x-post-auditor/)** | → **[Use the tool now](https://natyshi.github.io/x-post-auditor/)**  |
| Creada por **[@NatyShi_](https://x.com/NatyShi_)** - solopreneur, product builder. | Created by **[@NatyShi_](https://x.com/NatyShi_)** - solopreneur, product builder. |

---

# ¿Qué hace? | What does it do?

| Español | English |
|---|---|
| Pegás el texto de tu próximo post, marcás qué tipo de contenido es y qué incluye, y la herramienta te devuelve: | You paste the text of your next post, select what type of content it is and what it includes, and the tool returns: |
| • **Score de 0 a 100** según las señales que pondera el algoritmo real de X | • **Score from 0 to 100** based on the signals weighted by the real X algorithm |
| • **Señales detectadas** - qué está sumando y qué está restando puntos, con explicación de por qué | • **Detected signals** - what is adding and subtracting points, with an explanation of why |
| • **Recomendaciones accionables** - cambios concretos para mejorar el post antes de publicar | • **Actionable recommendations** - concrete changes to improve the post before publishing |
| • **Previsualización en tiempo real** - ves exactamente cómo se ve el post en el feed, dónde corta con "Mostrar más" y en qué zona de longitud estás (óptima / larga / truncada) | • **Real-time preview** - see exactly how the post looks in the feed, where it cuts with "Show more", and which length zone you're in (optimal / long / truncated) |
| Todo corre en tu navegador. No hay servidor, no se envían datos a ningún lado. | Everything runs in your browser. There is no server, and no data is sent anywhere. |

---

# ¿Por qué esto importa? | Why does this matter?

| Español | English |
|---|---|
| El algoritmo de X no distribuye todos los posts por igual. Prioriza contenido que genera **replies, dwell time y compartidos**, y penaliza links externos en el cuerpo, exceso de hashtags y patrones de engagement bait. | The X algorithm does not distribute all posts equally. It prioritizes content that generates **replies, dwell time, and shares**, and penalizes external links in the body, excessive hashtags, and engagement bait patterns. |
| Sin conocer esas reglas, podés estar publicando contenido que el propio algoritmo suprime antes de que llegue a tu audiencia. | Without knowing these rules, you may be publishing content that the algorithm itself suppresses before it reaches your audience. |

---

# Señales que analiza | Signals analyzed

| Señal | Lógica del algoritmo | Signal | Algorithm logic |
|---|---|---|---|
| **Link en el cuerpo** | Penalización del 30-50% de alcance - X retiene al usuario en la plataforma | **Link in body** | 30-50% reach penalty - X keeps the user on the platform |
| **Replies / CTA** | La señal de mayor peso. Más que likes o retweets | **Replies / CTA** | Highest weight signal. More than likes or retweets |
| **Video** | Activa el scorer VQV (video quality view) - dwell time máximo | **Video** | Triggers the VQV scorer (video quality view) - maximum dwell time |
| **Imagen** | Dispara la señal `photo_expand` | **Image** | Triggers the `photo_expand` signal |
| **Poll** | Genera dwell time + click obligatorio para votar | **Poll** | Generates dwell time + mandatory click to vote |
| **Hashtags** | El algoritmo 2025-2026 usa embeddings semánticos, no hashtags | **Hashtags** | The 2025-2026 algorithm uses semantic embeddings, not hashtags |
| **Longitud** | 60-280 chars = zona óptima. Más de 280 = truncado con "Mostrar más" | **Length** | 60-280 chars = optimal zone. More than 280 = truncated with "Show more" |
| **Tipo de post** | RT puro / RT con cita / reply / hilo tienen pesos distintos | **Post type** | Pure RT / quote RT / reply / thread have different weights |

---

# Tipos de contenido soportados | Supported content types

| Español | English |
|---|---|
| ✏️ Post original | ✏️ Original post |
| 💬 RT con cita | 💬 Quote RT |
| ↩️ Reply a otro post | ↩️ Reply to another post |
| 🧵 Hilo (primer tweet) | 🧵 Thread (first tweet) |
| 🔁 RT sin texto | 🔁 RT without text |

---

# Cómo usarla | How to use it

| Español | English |
|---|---|
| **Opción A - Online (recomendado):** Entrá al link de GitHub Pages de arriba. Funciona directo en el navegador. | **Option A - Online (recommended):** Open the GitHub Pages link above. Works directly in the browser. |
| **Opción B - Local:** | **Option B - Local:** |
| 1. Descargá el archivo `index.html` | 1. Download the `index.html` file |
| 2. Abrilo con doble click en cualquier navegador | 2. Open it with double click in any browser |
| 3. No necesita instalación ni conexión a internet (salvo la tipografía de Google Fonts) | 3. No installation or internet connection required (except for the Google Fonts typography) |

---

# Stack

| Español | English |
|---|---|
| HTML + CSS + JavaScript vanilla. Sin dependencias, sin frameworks, sin backend. Un solo archivo autocontenido. | HTML + CSS + vanilla JavaScript. No dependencies, no frameworks, no backend. A single self-contained file. |

---

# Fork / Contribuciones | Fork / Contributions

| Español | English |
|---|---|
| Podés forkear este repo y adaptarlo a tu caso. Ideas para extender: | You can fork this repo and adapt it to your use case. Ideas to extend it: |
| • Soporte para otros idiomas | • Support for other languages |
| • Integración con la API de X para analizar posts ya publicados | • Integration with the X API to analyze already published posts |
| • Historial de posts analizados (localStorage) | • History of analyzed posts (localStorage) |
| • Modo comparación A/B entre dos versiones del mismo post | • A/B comparison mode between two versions of the same post |
| Si lo usás o lo adaptás, un mention a [@NatyShi_](https://x.com/NatyShi_) es siempre bienvenido. 🙌 | If you use or adapt it, a mention to [@NatyShi_](https://x.com/NatyShi_) is always welcome. 🙌 |

---

# Fuente del algoritmo | Algorithm source

| Español | English |
|---|---|
| Basado en el código publicado por xAI en [github.com/xai-org/x-algorithm](https://github.com/xai-org/x-algorithm). Los pesos y señales reflejan el comportamiento documentado al momento de construcción de esta herramienta (mayo 2026). | Based on the code published by xAI at [github.com/xai-org/x-algorithm](https://github.com/xai-org/x-algorithm). The weights and signals reflect the documented behavior at the time this tool was built (May 2026). |

---

| Español | English |
|---|---|
| *Construido con obsesión por el producto y sin presupuesto de ads. Así se hace.* | *Built with product obsession and no ads budget. That’s how it’s done.* |
