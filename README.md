# Examen de Primer Bimestre - Sistema de Recuperación de Información

**Autor:** Danny Constante  
**Institución:** Escuela Politécnica Nacional (EPN) - Facultad de Ingeniería en Sistemas (FIS)  
**Materia:** ICCD753 Recuperación de Información  
**Período:** 2026-A  

## Descripción del Proyecto
Este repositorio contiene la implementación de un Sistema de Recuperación de Información desarrollado en un Jupyter Notebook. El sistema indexa un corpus de documentos textuales (Rotten Tomatoes Movies and Critic Reviews Dataset) mediante representaciones vectoriales densas (embeddings) y recupera los documentos más relevantes para una consulta dada utilizando similitud coseno.

Como parte del **Desafío de Excelencia**, el cuaderno incluye una implementación comparativa entre dos modelos de embeddings de la librería `sentence-transformers`: un modelo ligero (`all-MiniLM-L6-v2`) y un modelo denso (`all-mpnet-base-v2`).

## Estructura del Repositorio
* `ConstanteDanny_ex1bim_ir26a.ipynb`: Jupyter Notebook principal que contiene el código ejecutable, las celdas de texto explicativas y las tablas con los resultados de las consultas.
* `README.md`: Este archivo con la información general y las instrucciones de ejecución.

## Instrucciones Mínimas de Ejecución

Para reproducir los resultados de este sistema de recuperación, se recomienda utilizar el entorno de **Kaggle**, ya que el código hace uso de rutas nativas para la carga del corpus público.

1. **Entorno:** Sube el archivo `ConstanteDanny_ex1bim_ir26a.ipynb` a un nuevo cuaderno de Kaggle.
2. **Corpus:** Asegúrate de hacer clic en "Add Input" y buscar el dataset público *"Rotten Tomatoes Movies and Critic Reviews Dataset"*.
3. **Aceleración de Hardware:** Dado que se generan embeddings con modelos neuronales profundos, dirígete a las opciones de sesión (Session Options) en la esquina superior derecha y activa el Acelerador **GPU T4x2**.
4. **Dependencias:** No es necesario instalar dependencias de forma externa. La **primera celda** del cuaderno contiene el comando de instalación de las librerías necesarias (`sentence-transformers`, `scikit-learn`, `pandas`, `numpy`).
5. **Ejecución:** Selecciona *Run All* para ejecutar el cuaderno desde el inicio. Las celdas están ordenadas secuencialmente desde el preprocesamiento hasta el benchmark de consultas.
