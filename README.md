# ☁️ VisioNet: Módulo de Visión Artificial para Estación Meteorológica 4.0
> **Proyecto Integrador Institucional:** "Eco-Intelligence" 

[![Python](https://img.shields.io/badge/Python-3.12+-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://www.python.org/)
[![OpenCV](https://img.shields.io/badge/OpenCV-4.x-5C3EE8?style=for-the-badge&logo=opencv&logoColor=white)](https://opencv.org/)
[![YOLOv8](https://img.shields.io/badge/YOLOv8-Ultralytics-0066FF?style=for-the-badge&logo=ultralytics&logoColor=white)](https://ultralytics.com/)
[![Etapa](https://img.shields.io/badge/Etapa-Evidencia_III__Final-orange?style=for-the-badge)](https://www.ispc.edu.ar/)

---

## 📝 Descripción del Proyecto
Este repositorio constituye el núcleo de procesamiento visual del proyecto **"Eco-Intelligence"**. Nuestra misión es integrar técnicas avanzadas de **Procesamiento Digital de Imágenes (PDI)** y modelos de **Deep Learning** para automatizar la detección, delimitación y clasificación morfológica de géneros nubosos y fenómenos atmosféricos. Este módulo actúa como un sensor virtual complementario de los dispositivos físicos de la Estación Meteorológica 4.0.

Implementado bajo la metodología pedagógica de **ABP (Aprendizaje Basado en Proyectos)**, el software transforma matrices de píxeles crudos en vectores de conocimiento accionable y predictivo a corto plazo para la comunidad de la Escuela PRoA Río Tercero y la región.

---

## 🗺️ Pipeline del Sistema (Flujo de Trabajo)
El framework de **VisioNet** procesa la información a través de las siguientes etapas secuenciales:

1. **Ingesta Eficiente:** Montaje y descarga optimizada del dataset en caché local mediante subprocesos del sistema.
2. **Preprocesamiento Avanzado (PDI):** Reducción dimensional (Escala de grises), realce de texturas y densidades (Ecualización de histograma) y remoción de ruido (Filtro Gaussiano).
3. **Segmentación Estructural:** Aislamiento de capas nubosas y contornos térmicos mediante operadores gradientes (Algoritmo de Canny).
4. **Inferencia Adaptativa:** Clasificación y localización multiclase en tiempo real utilizando redes neuronales convolucionales (**YOLOv8**).

---

## 📊 Dataset: CCSN Database
El entrenamiento y validación de los modelos se sustenta en la base de datos **Cirrus Cumulus Stratus Nimbus (CCSN)**.
* **Clasificación:** 11 géneros morfológicos de nubes estandarizados por la Organización Meteorológica Mundial (OMM).
* **Propósito:** Segmentación y reconocimiento predictivo de nubosidad para alertas de microclima.
* **Acceso de Origen:** [🔗 Kaggle CCSN Database](https://www.kaggle.com/datasets/mmichelli/cirrus-cumulus-stratus-nimbus-ccsn-database)

---

## 🛠️ Stack Tecnológico
* **Lenguaje Core:** Python 3.12+ (NumPy, Matplotlib, Yaml).
* **Visión Artificial:** OpenCV (`cv2`), Ultralytics (`YOLOv8`).
* **Entornos de Cómputo:** Google Colab (Aceleración de hardware por GPU Nvidia T4).
* **Gestión de Proyectos:** Metodología Ágil, Trello y GitHub de Control de Versiones.

---

## 👥 Equipo de Investigación & Desarrollo (VisioNet)

Desarrollado por estudiantes avanzados de la *Tecnicatura Superior en Ciencia de Datos e Inteligencia Artificial* del **ISPC**:

| Miembro del Equipo | Rol / Especialidad Principal | GitHub |
| :--- | :--- | :---: |
| <img src="https://github.com/Nieves862.png" width="40px;"/><br/>**VILLALBA**, Valeria Nieves | Product Owner / Docente Tecnológica | [🐙 Perfil](https://github.com/Nieves862) |
| <img src="https://github.com/PaoTes.png" width="40px;"/><br/>**TESTA**, Andrea Paola | Data Engineer / ETL Pipeline | [🐙 Perfil](https://github.com/PaoTes) |
| <img src="https://github.com/github.png" width="40px;"/><br/>**GARCIA**, Carlos | Computer Vision Researcher / PDI | [🐙 Perfil](https://github.com) |
| <img src="https://github.com/github.png" width="40px;"/><br/>**MORENO**, Raúl | Data Analyst / Statistical Validation | [🐙 Perfil](https://github.com) |
| <img src="https://github.com/AllendeNicolas.png" width="40px;"/><br/>**ALLENDE**, Nicolás | Backend Developer / MLOps Infrastructure | [🐙 Perfil](https://github.com/AllendeNicolas) |
| <img src="https://github.com/JEmanuelG.png" width="40px;"/><br/>**GUARAZ**, Emanuel | UX/UI Designer / Data Visualization | [🐙 Perfil](https://github.com/JEmanuelG) |
| <img src="https://github.com/Cdireni.png" width="40px;"/><br/>**DIRENI**, Carlos | QA Engineer / Technical Documentation | [🐙 Perfil](https://github.com/Cdireni) |

---

## 📂 Estructura General del Repositorio
```bash
├── .github/             # Configuraciones de entorno y tokens de seguridad
├── notebooks/           # Cuadernos de Google Colab (Evidencias de PDI, Canny e Inferencia)
├── src/                 # Módulos modulares de producción (.py) para la estación
├── dataset/             # Muestras indexadas y configuraciones de metadatos (data.yaml)
└── docs/                # Informes institucionales y metodologías ABP

---

© 2026 ISPC - Instituto Superior Politécnico Córdoba.






