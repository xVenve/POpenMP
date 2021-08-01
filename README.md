# OpenMP ![GitHub repo size](https://img.shields.io/github/repo-size/xVenve/POpenMP)

[Memoria](https://drive.google.com/file/d/1wxbVAIxdkZhOwiKphuojJ-F4dqZhjVoj/view?usp=sharing)

# 1. Objetivo

Esta práctica tiene como objetivo fundamental hacer el que los estudiantes se familiaricen con la optimización de programas secuenciales y con los modelos de programación paralela en
arquitecturas de memoria compartida. En concreto, la práctica se centrará en el desarrollo de software secuencial en el lenguaje de programación C++ (incluyendo las mejoras de C++17), así como en las técnicas de paralelismo mediante
el uso de OpenMP.


# 2. Descripción del proyecto

En esta práctica se construirá una aplicación de filtrado de imágenes. Se desarrollarán dos versiones: una versión secuencial y otra versión paralela. En las siguientes secciones se presentn los requisitos que deben cumplir con los programas desarrollados. Así mismo, se hará público un archivo binario con un programa ejectuable con la funcionalidad
requerida. Esto hará más fácil la comparación de resultados. 


## 2.1. Visión general

Se desarrollará una aplicación que aplica dos filtros sobre un conjunto de imágenes en formato BMP. El resultado será una nueva imagen en el mismo formato después de aplicar los mencionados filtros.

Para cada imagen se aplicarán los siguientes filtros:
  - Difusión gaussiana (Gaussian blur).
  - Operador de Sobel.

Se desarrollarán dos versiones distintas del programa:
  -  image-seq: Versión secuencial.
  -  image-par: Versión paralela.
  
La aplicación (image-seq o image-par) tomará 3 parámetros:
  -  Modo de ejecución.
  -  Directorio con imágenes de entrada.
  -  Directorio en el que dejar las imágenes de salida.
  
El modo de ejecución será uno de los siguientes:
  -  copy: No realiza ninguna transformación. Solamente copia los archivos.
  -  gauss: Aplica el filtro de suavizado gaussiano.
  -  sobel: Aplica el filtro de suavizado gaussiano y el operador de Sobel
