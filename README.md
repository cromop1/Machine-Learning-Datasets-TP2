<p align="center">
  <img src="https://i.imgur.com/fFnG9fe.png" width="100%">
</p>

<p align="center">
<img src="https://img.shields.io/badge/Trabajo%20Academico-ITS%20Villada-blue?style=for-the-badge">
</p>

<p align="center">

<img src="https://img.shields.io/badge/Python-3.10-blue?logo=python&logoColor=white">
<img src="https://img.shields.io/badge/Machine%20Learning-Model-green?logo=tensorflow&logoColor=white">
<img src="https://img.shields.io/badge/Dataset-MalFlow-orange?logo=databricks&logoColor=white">
<img src="https://img.shields.io/badge/Platform-Kaggle-20BEFF?logo=kaggle&logoColor=white">
<img src="https://img.shields.io/badge/Area-Cybersecurity-red?logo=hackthebox&logoColor=white">


</p>



<p align="center">
  <img src="https://i.imgur.com/RVGaecC.png" width="100%">
</p>

<div align="center">

# 📘 Índice

[Introducción](#-introducción)

[Objetivo](#-objetivo)

[Dataset Analizado](#-dataset-analizado)

[¿Qué predeciría el modelo?](#-qué-predeciría-el-modelo)

[Tipo de Machine Learning](#-qué-tipo-de-machine-learning-utilizaría)

[Features más relevantes](#-qué-features-serían-más-útiles)

</div>

<p align="center">
  <img src="https://i.imgur.com/RVGaecC.png" width="100%">
</p>

# 🔸 Introducción

En el campo de la **ciencia de datos y la ciberseguridad**, los datasets representan una herramienta fundamental para entrenar modelos de **Machine Learning** capaces de identificar patrones dentro de grandes volúmenes de información.

El análisis del tráfico de red permite detectar comportamientos anómalos, identificar posibles amenazas y mejorar los sistemas de seguridad dentro de infraestructuras informáticas modernas.

En esta actividad se analiza el dataset **MalFlow**, el cual contiene información sobre flujos de tráfico de red generados por distintas comunicaciones dentro de una red.

A partir de estos datos es posible entrenar modelos de aprendizaje automático capaces de diferenciar entre **tráfico legítimo y tráfico potencialmente malicioso**, permitiendo desarrollar sistemas de detección automatizada de amenazas.



<p align="center">
  <img src="https://i.imgur.com/zDTIHyR.png" width="100%" alt="Banner Proyecto Integrador 2025">
</p>

# 🔸 Objetivo

El objetivo de este trabajo es analizar cómo puede utilizarse un dataset de tráfico de red para entrenar un modelo de **Machine Learning**, evaluando diferentes aspectos del proceso de aprendizaje automático.

Entre los puntos principales se encuentran:

* Analizar qué tipo de predicción puede realizarse utilizando el dataset.
* Identificar qué tipo de algoritmo de Machine Learning resulta más adecuado.
* Determinar qué variables o **features** aportan mayor información para detectar patrones dentro del tráfico de red.

Este análisis permite comprender cómo los datos pueden utilizarse para construir sistemas capaces de **detectar amenazas informáticas dentro de redes digitales**.



<p align="center">
  <img src="https://i.imgur.com/zDTIHyR.png" width="100%" alt="Banner Proyecto Integrador 2025">
</p>

# 🔹 Dataset Analizado

El dataset analizado en esta actividad es **MalFlow**, disponible en la plataforma Kaggle.

🔗 Link del dataset
[https://www.kaggle.com/datasets/amester/malflow](https://www.kaggle.com/datasets/amester/malflow)

Este dataset contiene información sobre **flujos de tráfico de red**, donde cada registro representa una conexión entre dispositivos dentro de una red informática.

Entre las características registradas se incluyen:

* duración de la conexión
* cantidad de paquetes transmitidos
* volumen de datos enviados y recibidos
* puertos de origen y destino
* protocolo de comunicación

Estas variables permiten describir el comportamiento de cada conexión dentro de la red, lo que facilita el análisis de patrones de comunicación entre sistemas.


<p align="center">
  <img src="https://i.imgur.com/zDTIHyR.png" width="100%" alt="Banner Proyecto Integrador 2025">
</p>

# 🔸 ¿Qué predeciría el modelo?

Si se entrenara un modelo utilizando este dataset, el objetivo principal sería **predecir si un flujo de tráfico de red corresponde a actividad maliciosa o a tráfico legítimo**.

El modelo analizaría las diferentes características presentes en cada registro del dataset para identificar patrones que indiquen comportamientos sospechosos dentro de la red.

Este problema se clasifica como un **problema de clasificación**, ya que el modelo debe asignar cada flujo de red a una categoría específica.

Dependiendo de la estructura del dataset, también podría abordarse como un problema de **clasificación multiclase**, donde además de detectar tráfico malicioso se identifica el tipo específico de amenaza presente en la comunicación.



<p align="center">
  <img src="https://i.imgur.com/zDTIHyR.png" width="100%" alt="Banner Proyecto Integrador 2025">
</p>

# 🔸 ¿Qué tipo de Machine Learning utilizaría?

Para resolver este problema se utilizaría **Machine Learning supervisado**, debido a que el dataset contiene registros previamente etiquetados que indican si el tráfico corresponde a actividad normal o maliciosa.

En este enfoque, el modelo aprende a partir de ejemplos previamente clasificados, identificando relaciones entre las variables del dataset y su clasificación.

Entre los algoritmos más adecuados para este tipo de problema se encuentran:

* **Random Forest**
* **Gradient Boosting**
* **Decision Trees**
* **Support Vector Machines**

Estos algoritmos son especialmente eficaces al trabajar con **datos tabulares**, ya que permiten capturar relaciones complejas entre múltiples variables y manejar grandes volúmenes de datos de manera eficiente.



<p align="center">
  <img src="https://i.imgur.com/zDTIHyR.png" width="100%" alt="Banner Proyecto Integrador 2025">
</p>

# 🔸 ¿Qué features serían más útiles?

Las **features** más relevantes dentro de este dataset son aquellas que describen el comportamiento del flujo de red y la interacción entre dispositivos dentro de la infraestructura.

Entre las variables más importantes se encuentran:

* **Duración de la conexión**
* **Cantidad de paquetes transmitidos**
* **Cantidad de bytes enviados y recibidos**
* **Puertos de origen y destino**
* **Protocolo de red utilizado**

Estas características permiten identificar patrones asociados al tráfico malicioso, ya que muchos tipos de malware generan **comportamientos anómalos dentro de la red**, como conexiones repetitivas hacia servidores externos, uso de puertos poco comunes o transferencias de datos inusuales.

El análisis de estas variables permite entrenar modelos capaces de detectar **comportamientos sospechosos dentro de una red informática**.




<p align="center">
<img src="https://img.shields.io/badge/By_Bruno_Segura-blue?style=for-the-badge">
</p>




