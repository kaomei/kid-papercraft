<div align="center">

[简体中文](README.md) · [English](README.en.md) · [日本語](README.ja.md) · [한국어](README.ko.md) · [**Español**](README.es.md)

# 🎂 Kid Papercraft (Generador de Videos de Cumpleaños en Origami para Niños)

### Convierte el cumpleaños de cualquier niño en un mágico video de origami stop-motion de 30 segundos con populares héroes de animación.

Un Skill de IA de código abierto para creadores y familias. Ingresa el nombre, edad, foto o descripción del niño para generar 3 escenas de stop-motion optimizadas para **Gemini Omni Flash** con guiones de locución incluidos.

![Codex Skill](https://img.shields.io/badge/Codex-Skill-111827?style=flat-square)
![Gemini Omni Flash](https://img.shields.io/badge/Gemini-Omni%20Flash-6d28d9?style=flat-square)
![Duración del Video](https://img.shields.io/badge/Duración-30%20Segundos-0066ff?style=flat-square)
![5 IPs Populares](https://img.shields.io/badge/IPs-5%20Caricaturas%20Populares-f59e0b?style=flat-square)
![MIT License](https://img.shields.io/badge/License-MIT-16a34a?style=flat-square)

<br/>

<img src="assets/readme/hero-cover.png" alt="Vista previa de Kid Papercraft" width="800">

<br/>

Ideal para: **Saludos de cumpleaños personalizados, celebraciones familiares, videos cortos para TikTok / Instagram Reels / YouTube Shorts**.

</div>

---

## ✨ Características Principales

- 🎭 **5 Mundos Animados en Origami**: Bob Esponja, Peppa Pig, Ultraman, Paw Patrol y Doraemon con estética de papel artesanal.
- ⏱️ **Estructura Narrativa de 3 Actos (30 Segundos = 3 Clips de 10s)**:
  - **Acto 1 (0–10s) Entrada Creativa**: Los personajes salen de escenarios de papel doblado con divertidas animaciones.
  - **Acto 2 (10–20s) Celebración de Cumpleaños**: Los personajes sostienen un pastel brillante y un cartel con el avatar de origami del niño.
  - **Acto 3 (20–30s) Buenos Hábitos con Amor**: Animaciones tiernas recordando cepillarse los dientes 🪥, dormir a tiempo 😴 y comer sano 🍽️.
- 👶 **Avatar Personalizado del Niño**: Admite descripciones físicas y fotos como Reference Image (Imagen de Referencia).
- 📐 **Formatos Adaptables**: `9:16` (Vertical para Shorts/Reels/TikTok) y `16:9` (Horizontal para TV/Tablets).
- 🎙️ **Guiones de Voz y Subtítulos**: Textos adaptados a la personalidad de cada personaje para la edición final.

---

## 🎬 5 Franquicias de Animación Compatibles

| # | Caricatura / IP | Personajes Principales | Escenario de Origami |
|:---:|:---|:---|:---|
| 🧽 | **Bob Esponja** | Bob Esponja y Patricio | Casa de Piña de Fondo de Bikini y arrecifes de papel |
| 🐷 | **Peppa Pig** | Peppa y George | Colinas de hierba y charcos de barro de papel |
| ⭐ | **Ultraman** | Héroe Chibi y pequeño monstruo amigo | Ciudad miniatura de papel al atardecer |
| 🐶 | **Paw Patrol** | Chase y Marshall | Plaza del pueblo de rescate y caseta de papel |
| 🤖 | **Doraemon** | Doraemon y Nobita | Habitación acogedora con inventos mágicos de papel |

---

## 📋 Ejemplo de Salida (Bob Esponja 5to Cumpleaños)

<div align="center">
  <a href="assets/readme/spongebob-birthday-demo.mp4">
    <img src="assets/readme/spongebob-birthday-demo.gif" alt="Demostración de Origami Bob Esponja" width="750">
  </a>
  <p><em>🎬 Tema de Bob Esponja · Demostración de Video en Origami Stop-Motion de 30 Segundos（<strong>Haz clic en el GIF para abrir el video en HD con sonido</strong>）</em></p>
</div>

### 🎬 Clip 1: Entrada Creativa (0–10s)
```text
Charming stop-motion animation of an origami ocean world. Beautifully textured colored paper cutouts of SpongeBob SquarePants and Patrick Star made of origami, popping out of a folding paper pineapple house and a paper rock, doing a silly dance and bumping into each other, laughing joyfully. Paper bubbles float up around them. Warm organic lighting, tactile paper textures, gentle camera pan, soft pastel color palette, whimsical and cozy atmosphere.
```

### 🎬 Clip 2: Celebración de Cumpleaños (10–20s)
```text
Charming stop-motion animation in a colorful origami underwater party room with paper coral and seaweed decorations. Beautifully textured colored paper cutouts of origami SpongeBob SquarePants and Patrick Star wearing paper party hats and blowing paper horns standing together with a cute small origami paper child (a cheerful boy with a round face, short black hair, black-rimmed glasses, and a cozy yellow hoodie), all gathered around a large origami birthday cake with 5 paper candles glowing softly. The characters hold up a folding paper banner that reads "Happy Birthday Lele!". Paper confetti and tiny origami stars fall gently from above. Warm organic lighting, tactile paper textures, gentle camera pan, soft pastel color palette, whimsical and cozy atmosphere.
```

### 🎬 Clip 3: Buenos Hábitos (20–30s)
```text
Charming stop-motion animation montage in SpongeBob's origami pineapple house interior. Beautifully textured colored paper cutouts showing three quick adorable scenes: First, the cheerful origami SpongeBob cheerfully brushing teeth with a tiny origami toothbrush, with sparkles of paper glitter around the smile. Then, the cheerful origami SpongeBob yawning cutely and tucking into a cozy origami paper bed with a paper star nightlight. Finally, the cheerful origami SpongeBob happily eating from a colorful origami paper plate with tiny paper vegetables and rice. Each scene transitions with a gentle paper fold wipe. Warm organic lighting, tactile paper textures, gentle camera pan, soft pastel color palette, whimsical and cozy atmosphere.
```

---

## 🛠️ Flujo de Trabajo (Workflow)

```mermaid
flowchart LR
    A[1. Elegir IP y Formato] --> B[2. Ingresar Datos/Foto del Niño]
    B --> C[3. El Skill Genera 3 Prompts]
    C --> D[4. Generar Video en Omni Flash]
    D --> E[5. Unir y Agregar Voz en CapCut]
```

---

## 📦 Instalación y Uso

```bash
git clone https://github.com/kaomei/kid-papercraft.git
cd kid-papercraft

# Para Antigravity / Gemini CLI
cp -R skills/kid-papercraft ~/.gemini/config/skills/kid_papercraft

# Para Codex CLI
cp -R skills/kid-papercraft "${CODEX_HOME:-$HOME/.codex}/skills/kid_papercraft"
```

Invocar en la conversación:
```text
¡Ayúdame a crear un video de cumpleaños en origami para mi hijo!
```

---

## ⚠️ Descargo de Responsabilidad y Derechos de PI (Disclaimer)

1. **Proyecto No Oficial**: Este repositorio de código abierto (`kid-papercraft`) proporciona plantillas de ingeniería de prompts y habilidades de flujo de trabajo. **Es un proyecto independiente sin afiliación, patrocinio ni respaldo de ningún estudio de animación o titular de marca**.
2. **Propiedad Intelectual**: Todos los personajes animados, marcas registradas y nombres (incluidos Bob Esponja, Peppa Pig, Ultraman, Paw Patrol, Doraemon, etc.) pertenecen a sus respectivos creadores y titulares de derechos de autor.
3. **Uso Permitido**: Las plantillas se proporcionan exclusivamente para estudio personal, investigación tecnológica, exploración artística y **videos de felicitación familiar de carácter no comercial**.

---

## 🤝 Contribuciones

¡Las solicitudes de extracción (PR), nuevas plantillas de IP y optimizaciones de prompts son bienvenidas!

Si este proyecto te ayudó a crear un momento especial, **¡dale una Star ⭐️ para apoyar a kaomei (烤妹儿)!**

## 📄 Licencia

[MIT License](LICENSE) © 2026 [kaomei](https://github.com/kaomei)
