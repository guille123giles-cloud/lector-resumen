# 🎧 Lector IA: OCR & Text-to-Speech Engine

![Python](https://img.shields.io/badge/Python-3.9+-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?style=for-the-badge&logo=Streamlit&logoColor=white)
![Tesseract](https://img.shields.io/badge/Tesseract--OCR-blue?style=for-the-badge)

**Lector IA** es una herramienta potente y minimalista diseñada para convertir material de estudio en audiolibros personalizados. Combina reconocimiento óptico de caracteres (OCR) para leer fotos de apuntes y síntesis de voz (TTS) de alta fidelidad, facilitando el estudio dinámico y la accesibilidad.

---

## 🚀 Características Principales

* **Extracción Multiformato:** Procesa archivos PDF, Word (`.docx`), PowerPoint (`.pptx`) y archivos de imagen.
* **Motor OCR Integrado:** Digitaliza texto de fotos y capturas (`.jpg`, `.png`, `.jpeg`) utilizando **Tesseract OCR**, optimizado para el idioma español.
* **Voces Neuronales:** Utiliza la tecnología de **Microsoft Edge TTS** para ofrecer voces humanas y naturales con acentos regionales (Argentina, España, México).
* **Procesamiento Asíncrono:** Maneja textos extensos de manera eficiente mediante fragmentación de texto y `asyncio`, evitando bloqueos en la interfaz.
* **Ajustes de Lectura:** Control total sobre la velocidad de reproducción (desde 0.5x hasta 2.0x) y selección de tono de voz.

---

## 🛠️ Stack Tecnológico

* **Frontend & Web App:** [Streamlit](https://streamlit.io/)
* **OCR (Optical Character Recognition):** [PyTesseract](https://github.com/madmaze/pytesseract)
* **TTS (Text-to-Speech):** [Edge-TTS](https://github.com/rany2/edge-tts)
* **Lógica de Procesamiento:** Python (Asyncio, PIL, Textwrap, Base64)

---

## 📦 Instalación y Configuración

Para correr este proyecto de forma local, seguí estos pasos:

1.  **Cloná el repositorio:**
    ```bash
    git clone [https://github.com/tu-usuario/ocr-async-tts-engine.git](https://github.com/tu-usuario/ocr-async-tts-engine.git)
    cd ocr-async-tts-engine
    ```

2.  **Instalá las dependencias de Python:**
    ```bash
    pip install -r requirements.txt
    ```

3.  **Configuración de Tesseract OCR:**
    * **Windows:** Descargá e instalá Tesseract. Asegurate de que la ruta en el código coincida con `C:\Program Files\Tesseract-OCR\tesseract.exe`.
    * **Linux/Mac:** Instalá el motor mediante el gestor de paquetes (ej: `sudo apt install tesseract-ocr tesseract-ocr-spa`).

4.  **Iniciá la aplicación:**
    ```bash
    streamlit run app.py
    ```

---

## 💡 Modo de Uso

1.  **Carga de datos:** Seleccioná si querés subir un archivo (PDF, Word, Imagen) o pegar el texto directamente.
2.  **Configuración:** En la barra lateral (o sección de ajustes), elegí el acento de la voz y la velocidad que prefieras.
3.  **Conversión:** Hacé clic en el botón **"🔊 GENERAR AUDIO"**. Verás una barra de progreso mientras la IA procesa el texto.
4.  **Descarga:** Una vez finalizado, podés reproducir el audio directamente en la web o descargarlo como un archivo `.mp3` para escucharlo offline.

---
*Desarrollado con ❤️ como herramienta de apoyo al estudio y productividad.*
