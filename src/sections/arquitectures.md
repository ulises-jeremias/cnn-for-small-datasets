# Modelos

----

Para resolver este problema vamos a analizar dos modelos:

- DenseNet <!-- .element: class="fragment" -->
- Prototypical Networks <!-- .element: class="fragment" -->

---

<!-- .slide: style="text-align: left" -->

## DenseNet

- Estado del Arte en la clasificación de imagenes con CNN
- No diseñado especificamente para datasets pequeños
    - **puede manejarlos con baja tasa de error**

----

DenseNet funciona concatenando los mapas de características de un bloque convolucional con los mapas de características de todos los bloques convolucionales anteriores y usando este valor como entrada para el siguiente bloque convolucional.

<center>
![DenseNet](static/DenseConnectivity.png)
<!-- .element: style="width: 75%; border: none" -->
</center>

----

Cada bloque convolucional recibe todo el conocimiento colectivo de las capas anteriores manteniendo el estado global de la red a la que se puede acceder

----

<!-- .slide: style="text-align: left" -->

## Ventajas

- Mejor eficiencia de parámetros
<small>No es necesario volver a aprender los mapas de características redundantes</small>

- Fortalecen la propagación de características

- Fomentan la reutilización de características

----

![DenseNet](static/DenseNet.png)
<!-- .element: style="border: none" -->

---

## Prototypical Networks

----

<!-- .slide: style="text-align: left" -->

### Prototypical Networks

Modelo de meta-learning para el problema de la clasificación de pocos "disparos".

----

Few shot learning generalmente se mide por su rendimiento en tareas de clasificación n-shot y k-way.

----

<!-- .slide: style="text-align: left" -->

### Algoritmo

![](static/protonets.png)

----

<!-- .slide: style="text-align: left" -->

### Algoritmo

- Un modelo es dado de una muestra de consulta que pertenece a una clase nueva nunca antes vista.

- Se proporciona un conjunto de soporte que consta de n ejemplos, cada uno de k diferentes clases no vistas.

- Determinar a qué clase de conjunto de soporte pertenecen las muestras de consulta.

----

<!-- .slide: style="text-align: left" -->

Los esquemas para algunas tareas de few shot classification, como las Prototypical Nets, también pueden ser útiles para entrenar pequeños conjuntos de datos donde se conocen todas las clases.
