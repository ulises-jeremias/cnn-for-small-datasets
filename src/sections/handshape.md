## Reconocimiento de forma de mano

----

### Conjuntos de datos

- <small>**LSA16**, 16 formas de mano del Lenguaje de Señas Argentino (LSA) para un total de 800 imágenes de tamaño 32x32.</small>

- <small>**RWTH** está compuesto por una selección de imágenes de tamaño 132x92 recortadas de videos de los intérpretes de lenguaje de señas en la estación de televisión pública alemana PHOENIX.De un total de 45 clases no quedamos con aquellas que cuentan con más de 20 ejemplos.</small>

- <small>**CIARP** contiene 6000 imágenes de tamaño 38x38 adquiridas por una cámara de un solo color. Las imágenes fueron etiquetadas manualmente y corresponden a 10 clases de gestos con las manos.</small>

----

### Conjuntos de datos

![datasets](static/datasets.png)
<!-- .element: style="width: 75%" -->

----

## Pasos

----

### Data Augmentation

- Flip
- Rotación (10 a 30 grados)
- Redimensionar (10% o 20% en ancho y alto)

----

### Resultados

![results](static/results.png)

----

<!-- .slide: style="text-align: left" -->

### ¿Qué sigue?

- Comparar con otros datasets
<small>Entender mejor la relación entre los modelos y la complejidad del conjunto de datos</small>

- Comparar modelos previamente entrenados

- Investigar métodos que aprovechen datos no etiquetados.

- Combinar conjuntos de datos para aumentar la muestra.

- Data augmentation.