# 🐢 SistemaVozText-to-Speech

<div align="center">

<img width="220" src="https://cdn-icons-png.flaticon.com/512/4712/4712109.png" />

### Sistema avanzado de Text-to-Speech con Inteligencia Artificial 🚀

<p align="center">
  <b>TorToiSe TTS</b> es un modelo de síntesis de voz basado en IA diseñado para generar voces ultra realistas, clonación de voz y audio natural utilizando modelos autoregresivos y difusión.
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Python-3.9+-blue?style=for-the-badge&logo=python" />
  <img src="https://img.shields.io/badge/PyTorch-AI-red?style=for-the-badge&logo=pytorch" />
  <img src="https://img.shields.io/badge/TTS-Voice%20Cloning-purple?style=for-the-badge" />
  <img src="https://img.shields.io/badge/CUDA-GPU-success?style=for-the-badge&logo=nvidia" />
  <img src="https://img.shields.io/badge/License-MIT-green?style=for-the-badge" />
</p>

</div>

---

# 📖 Descripción

TorToiSe es un sistema avanzado de generación de voz mediante inteligencia artificial enfocado en:

- 🎤 Clonación avanzada de voz
- 🧠 Generación de voces ultra realistas
- 🎭 Soporte multi-speaker
- 🔊 Audio natural y expresivo
- ⚡ API programable en Python
- 🎲 Generación de voces aleatorias
- 🛡️ Detector de audio IA

El proyecto combina Transformers autoregresivos y modelos de difusión para producir síntesis de voz de alta calidad.

---

# ✨ Características

✅ Clonación de voz mediante clips de referencia  
✅ Generación de voz realista y expresiva  
✅ Soporte para múltiples voces  
✅ Modelos autoregresivos + difusión  
✅ API Python para integración  
✅ Generación de voces aleatorias  
✅ Lectura de textos largos  
✅ Ingeniería de prompts  
✅ Compatible con GPU NVIDIA  
✅ Compatible con Windows, Linux y macOS  

---

# 🏗️ Arquitectura

```bash
tortoise-tts/
│
├── tortoise/
│   ├── api.py
│   ├── do_tts.py
│   ├── read.py
│   ├── models/
│   └── utils/
│
├── voices/
├── results/
├── requirements.txt
└── setup.py
```

---

# 🧠 Tecnologías Utilizadas

| Tecnología | Uso |
|------------|-----|
| Python | Lenguaje principal |
| PyTorch | Deep Learning |
| Transformers | Procesamiento de voz |
| CUDA | Aceleración GPU |
| HuggingFace | Modelos IA |
| UnivNet | Vocoder neural |
| NumPy | Procesamiento numérico |

---

# 🚀 Instalación

## 📋 Requisitos

- Python 3.9+
- GPU NVIDIA recomendada
- CUDA instalado
- Git

---

## 📥 Clonar repositorio

```bash
git clone https://github.com/neonbjb/tortoise-tts.git
cd tortoise-tts
```

---

## 📦 Instalar dependencias

```bash
pip install -r requirements.txt
```

---

## ⚙️ Instalar proyecto

```bash
python setup.py install
```

---

# 🖥️ Instalación en Windows

Se recomienda usar Conda.

```bash
conda install -c conda-forge pysoundfile
```

---

# 🍎 Instalación en macOS

```bash
brew install ffmpeg
```

---

# ▶️ Uso Básico

## Generar voz

```bash
python tortoise/do_tts.py --text "Hola mundo" --voice random --preset fast
```

---

# 📚 Leer textos largos

```bash
python tortoise/read.py --textfile libro.txt --voice random
```

---

# 🎲 Voces Aleatorias

```bash
python tortoise/do_tts.py --text "Esta voz fue generada por IA" --voice random
```

---

# 🎤 Voces Personalizadas

## Pasos

1. Crear carpeta en `voices/`
2. Agregar clips `.wav`
3. Ejecutar:

```bash
python tortoise/do_tts.py --voice mi_voz
```

---

# 🧩 API en Python

```python
from tortoise.api import TextToSpeech
from tortoise.utils.audio import load_audio

tts = TextToSpeech()

audio = tts.tts_with_preset(
    "Hola, esta es una demostración",
    preset="fast"
)
```

---

# 🎛️ Presets Disponibles

| Preset | Descripción |
|---------|-------------|
| ultra_fast | Máxima velocidad |
| fast | Balance velocidad/calidad |
| standard | Calidad estándar |
| high_quality | Mejor calidad |

---

# 🎭 Ingeniería de Prompts

```text
[I am very sad,] Please help me.
```

El texto entre corchetes modifica la emoción sin pronunciarse.

---

# 🎤 Consejos para Voces

✅ Clips limpios  
✅ Sin ruido  
✅ WAV 22050 Hz  
✅ Mínimo 3 clips  
✅ Audios de 10 segundos  

---

# 🧪 Ejemplos

## Voz aleatoria

```bash
python tortoise/do_tts.py --voice random
```

## Leer archivo

```bash
python tortoise/read.py --textfile story.txt
```

## Detectar audio IA

```bash
python tortoise/is_this_from_tortoise.py --clip=audio.wav
```

---

# 📊 Rendimiento

| Hardware | Velocidad |
|-----------|-----------|
| RTX 4090 | Excelente |
| RTX 3090 | Muy rápida |
| RTX 2060 | Buena |
| CPU | Muy lenta |

---

# 🛡️ Consideraciones Éticas

TorToiSe incluye advertencias relacionadas con:

- Deepfakes
- Clonación de voz
- Suplantación de identidad
- Audio sintético

También incorpora herramientas de detección de voz generada por IA.

---

# 📷 Demo

<p align="center">
  <img src="https://raw.githubusercontent.com/neonbjb/tortoise-tts/main/imgs/tortoise.png" width="700">
</p>

---

# 📈 Casos de Uso

- 🎙️ Audiolibros
- 🤖 Asistentes virtuales
- 🎮 NPCs con voz IA
- 🎬 Doblaje automático
- 🎧 Podcasts
- 📚 Educación
- 🎵 Multimedia
- 🧠 Investigación IA

---

# 🔥 Funciones Avanzadas

- Voice Latent Manipulation
- Prompt Engineering
- Voice Mixing
- Multi-Speaker Conditioning
- Diffusion Decoding
- Audio Classification

---

# 👨‍💻 Autor

## Brandon Blackwell (neonbjb)

Creador principal de TorToiSe TTS.

---

# 🤝 Contribuciones

```bash
Fork 🍴
Clone 📥
Commit 💾
Push 🚀
Pull Request 🔥
```

Las contribuciones son bienvenidas.

---

# ⭐ Roadmap

- [x] Clonación de voz
- [x] API Python
- [x] Voces aleatorias
- [x] Detector IA
- [ ] Interfaz web
- [ ] Optimización GPU
- [ ] App escritorio

---

# 📜 Licencia

```text
MIT License © TorToiSe TTS
```

---

<div align="center">

## 🐢 TorToiSe TTS

### Inteligencia artificial para síntesis de voz ultra realista 🎤

⭐ No olvides dejar una estrella al proyecto ⭐

</div>
