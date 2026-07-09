# Prototipado de Clasificación Automática de Discurso de Odio y Sarcasmo

Este repositorio contiene el código, los conjuntos de datos y la documentación del **Trabajo de Fin de Grado (TFG)** orientado al desarrollo de un pipeline de procesamiento de lenguaje natural (PLN) para la detección y moderación de contenido nocivo en entornos digitales.

* **Autor:** Adrián Tomás Herrera Darias
* **Tutores:** Dagoberto Castellanos Nieves y Luis García Forte
* **Institución:** Universidad de La Laguna

---

## 📂 Estructura del Repositorio

El proyecto se organiza en las siguientes carpetas principales:

*   **`Cuaderno/`**: Contiene todo el código fuente, scripts y cuadernos de Jupyter utilizados para el flujo de ingeniería de características, el entrenamiento de las arquitecturas y las pruebas de evaluación cuantitativa y cualitativa.
*   **`Data/`**: Espacio destinado al almacenamiento local y procesamiento de los conjuntos de datos experimentales utilizados en el prototipo.

---

## 🤖 Modelos Seleccionados

En este proyecto se implementaron y evaluaron diferentes arquitecturas basadas en *Transformers* (codificadores) accesibles a través de Hugging Face:

*   **RoBERTa Base (Español):** [bertin-project/bertin-roberta-base-spanish](https://huggingface.co/bertin-project/bertin-roberta-base-spanish)
*   **ELECTRA Base Discriminator:** [google/electra-base-discriminator](https://huggingface.co/google/electra-base-discriminator)
*   **ELECTRA Large NLI EFL HatEval:** [ChrisZeng/electra-large-discriminator-nli-efl-hateval](https://huggingface.co/ChrisZeng/electra-large-discriminator-nli-efl-hateval)
*   **DistilBERT Base Multilingual Cased:** [distilbert/distilbert-base-multilingual-cased](https://huggingface.co/distilbert/distilbert-base-multilingual-cased)

---

## 📊 Conjuntos de Datos (Corpus)

Los datos crudos y procesados necesarios para replicar los experimentos se encuentran alojados en la carpeta `Data/`, mapeando los siguientes repositorios oficiales:

*   **Toxic_es:** [dolfsai/toxic_es](https://huggingface.co/datasets/dolfsai/toxic_es) — Detección multiclase de toxicidad e insultos en español.
*   **Id-x-sarcasm:** [savioruz/id-x-sarcasm](https://huggingface.co/datasets/savioruz/id-x-sarcasm) — Estudio del lenguaje no auténtico y estructuras irónicas.
*   **Toxic_conversations_50k:** [toxic_conversations_50k](https://huggingface.co/datasets/toxic_conversations_50k) — Análisis masivo para la moderación y control cualitativo de sesgos.

---

## 🚀 Ejecución en Google Colab

No requiere ninguna instalación local. Todos los entornos experimentales y cuadernos de código interactivos situados en la carpeta `Cuaderno/` incluyen un enlace directo para ser ejecutados en la nube de forma inmediata:

1. Navega a la carpeta `Cuaderno/`.
2. Selecciona el archivo `.ipynb` que deseas auditar.
3. Haz clic en el botón **"Open in Colab"** integrado en la cabecera del archivo para abrir y ejecutar las celdas de entrenamiento o evaluación utilizando el entorno de GPU gratuito proporcionado por Google.
