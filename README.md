# Aprendizaje No Supervisado – Rostros de Olivetti

Este repositorio forma parte del proyecto del curso de Machine Learning que cursé en la SIAFI, desarrollado dentro del Curso Propedéutico.

El proyecto utiliza el conjunto de datos de rostros de Olivetti para explorar técnicas de aprendizaje no supervisado.
El trabajo se documenta paso a paso mediante cuadernos de Jupyter.

Temas principales abordados:
- Carga y preprocesamiento de datos
- Agrupamiento de K-Medias
- Reducción de dimensionalidad mediante PCA
- Modelos de Mezcla Gaussiana
- Detección básica de anomalías

Todos los resultados y explicaciones se incluyen directamente en los cuadernos.

## **Proyecto 1 — Clustering (K-Means)**
[`PROYECTO_A2B_1.ipynb`](PROYECTO_A2B_1.ipynb)  
Explora el uso de K-Means para agrupar imágenes del dataset Olivetti Faces.

> **Project description**  
>  
> The classic Olivetti faces dataset contains 400 grayscale 64 × 64–pixel images of faces. 
> Each image is flattened to a 1D vector of size 4,096. Forty different people were photographed (10 times each), and the usual 
> task is to train a model that can predict which person is represented in each picture. 
> Load the dataset using the `sklearn.datasets.fetch_olivetti_faces()` function, then split it into a training set, a validation 
> set, and a test set (note that the dataset is already scaled between 0 and 1). Since the dataset is quite small, you will probably 
> want to use stratified sampling to ensure that there are the same number of images per person in each set. Next, cluster the 
> images using k-means, and ensure that you have a good number of clusters (using one of the techniques discussed in this chapter). 
> Visualize the clusters: do you see similar faces in each cluster? Comment and explain what you observe.



## **Proyecto 2 — Generative Models (GMM)**  
[`PROYECTO_A2B_2.ipynb`](PROYECTO_A2B_2.ipynb)  
Entrena un modelo de mezcla gaussiana para generación de rostros y detección de anomalías.

> **Project description**  
>  
> Train a Gaussian mixture model on the Olivetti faces dataset. To speed up the algorithm, you should probably
> reduce the dataset’s dimensionality (e.g., use PCA, preserving 99% of the variance). 
> Use the model to generate some new faces (using the `sample()` method), and visualize them (if you used PCA, you will
> need to use its `inverse_transform()` method). Try to modify some images (e.g., rotate, flip, darken)
> and see if the model can detect the anomalies (i.e., compare the output of the `score_samples()` method for normal images and for anomalies).  

