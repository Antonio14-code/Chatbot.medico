🩺 Proyecto de Diagnóstico Asistido con IA

🚀 Descripción
La aplicación permite:
- 📂 Leer PDFs médicos almacenados en Google Cloud Storage.
- 💻 Subir archivos locales (ej. análisis de sangre) desde Google Colab.
- 📑 Extraer texto automáticamente de los documentos usando PyMuPDF (fitz).
- 🤖 Consultar al modelo Gemini / Vertex AI con base en la información de los documentos.
- 🩺 Obtener respuestas clínicas y sugerencias de diagnóstico de forma asistida.

🛠️ Tecnologías utilizadas
- Python 3.8+
- Google Cloud Storage (GCS)
- Vertex AI / Gemini (modelos generativos de Google)
- LangChain para la integración con LLMs
- PyMuPDF (fitz) para la lectura de PDFs
- Google Colab para pruebas con archivos locales

📂 Flujo de trabajo
- 📥 El sistema descarga PDFs desde GCS o permite subir archivos locales.
- 📑 Se extrae todo el texto de los documentos médicos.
- 🧠 Se construye un prompt enriquecido con la información base (síntomas) y los documentos del usuario.
- 🤖 Se consulta al modelo Gemini ajustando parámetros como temperature, top_p y máximo de tokens.
- 🩺 El asistente devuelve interpretaciones, diagnósticos y posibles tratamientos.

⚙️ Requisitos previos
- Tener un proyecto activo en Google Cloud Platform (GCP).
- Contar con un Bucket en GCS para almacenar los PDFs clínicos.
- Configurar la API Key de Google Generative AI / Vertex AI.
- Instalar las dependencias (LangChain, PyMuPDF, Google Cloud SDK, etc.).

📑 Ejemplos de uso
- Interpretación de exámenes de sangre subidos por el usuario.
- Responder preguntas como:
  * "¿Qué tratamiento hacer con la Influenza A H1N1?"
  * "¿Qué hacer si un niño de 5 años tiene dolor abdominal?"
  * "¿Cuál es el tratamiento recomendado para alergias graves?"
