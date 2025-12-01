# 🏥 Modelado Espacio-Temporal de Urgencias Respiratorias en Chile

![Python](https://img.shields.io/badge/Python-3.10%2B-blue)
![TensorFlow](https://img.shields.io/badge/TensorFlow-2.x-orange)
![Status](https://img.shields.io/badge/Status-Finalizado-success)
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1ZXD6uYnlMKP-Zp6LxS8MoIvsU5VyGocA?usp=sharing)

> **Proyecto Final de Curso / Deep Learning:** Predicción de demanda y Clustering espacial mediante redes LSTM híbridas y Aprendizaje Contrastivo (Triplet Loss).

## 📄 Documentación
* 📘 **[Leer Informe Técnico Completo (PDF)](docs/Informe_Final_Hinostroza_Yanine.pdf)**
* 🎬 **[Ver Presentación del Proyecto (YOUTUBE)](https://www.youtube.com/watch?v=sleZWxBlpD8)**

## 📌 Contexto y Problemática
El sistema de salud enfrenta saturaciones críticas estacionales. El desafío técnico principal no es solo la predicción temporal, sino la **heterogeneidad territorial**:
* Comunas vecinas no siempre se comportan igual.
* Comunas distantes (ej. Norte y Sur) pueden tener dinámicas idénticas por factores latentes.

## 🚀 Solución: Pipeline Híbrido
Diseñamos una arquitectura de Deep Learning con dos ramas simultáneas:
1.  **Rama Predictiva (LSTM):** Captura secuencias temporales complejas.
2.  **Rama Contrastiva (Triplet Loss):** Aprende un *embedding* (huella digital) de cada comuna.

## 📊 Hallazgo Clave: El Clúster Norte-Sur
El modelo descubrió automáticamente el **Clúster 4**, agrupando a **Antofagasta** y **Coyhaique**.
* A pesar de estar a >2.000 km, ambas comparten identidad de "Zona Extrema Aislada".
* Esto valida que la similitud sanitaria trasciende la geografía física.

## 👥 Autores
* **Bryan Hinostroza**
* **Alan Yanine**

---
_Proyecto realizado para la Universidad Técnica Federico Santa María (2025)._
