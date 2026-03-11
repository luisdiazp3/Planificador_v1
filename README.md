# 📚 Planificador de Sesiones de Aprendizaje

Aplicación web desarrollada con **Streamlit** que utiliza inteligencia artificial (modelo **LLaMA 3 70B** vía **Groq**) para generar propuestas de sesiones de aprendizaje para docentes del sistema educativo peruano, alineadas al Currículo Nacional de Educación Básica (CNEB).

---

## ✨ Funcionalidades

- Generación automática de sesiones de aprendizaje con secuencia didáctica completa (inicio, desarrollo y cierre)
- Selección de nivel educativo, grado, área curricular y competencias del CNEB
- Incorporación de enfoques transversales
- Rúbrica de evaluación en formato de tabla
- Descarga de la sesión generada en formato **Word (.docx)**

---

## 🚀 Cómo ejecutar localmente

### 1. Clonar el repositorio
```bash
git clone https://github.com/tu-usuario/planificador.git
cd planificador
```

### 2. Crear entorno virtual e instalar dependencias
```bash
python3 -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
```

### 3. Configurar la clave de API de Groq
Crea el archivo `.streamlit/secrets.toml`:
```toml
GROQ_API_KEY = "gsk_tu_clave_aqui"
```
> Obtén tu clave gratuita en [console.groq.com](https://console.groq.com)

### 4. Ejecutar la aplicación
```bash
streamlit run Planificador_1.py
```

La app estará disponible en: `http://localhost:8501`

---


## 🛠️ Tecnologías utilizadas

| Tecnología | Uso |
|-----------|-----|
| [Streamlit](https://streamlit.io) | Interfaz web |
| [LangChain](https://langchain.com) | Orquestación de LLM |
| [Groq](https://groq.com) | Inferencia ultrarrápida del modelo LLaMA 3 |
| [LLaMA 3 70B](https://llama.meta.com) | Modelo de IA generativa |
| [python-docx](https://python-docx.readthedocs.io) | Generación de archivos Word |

---

## 📋 Requisitos

- Python 3.10+
- Clave API de Groq (gratuita)

---

## 📄 Licencia

Desarrollado para uso educativo en el marco del sistema educativo.
