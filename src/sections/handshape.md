## Reconocimiento de forma de mano

----

### Conjuntos de datos

![datasets](static/datasets.png)
<!-- .element: style="width: 75%" -->

----

<!-- .slide: style="text-align: left;" -->

## LSA16
<small style="margin-top: -25px;"><em>
Lenguaje de Señas Argentino (LSA)
</em></small>      

<div class="row" style="font-size: 2.53rem;">
    <div class="col-6">
        ![lsa16](static/lsa16.png)
        <!-- .element: style="width: 75%;" -->
    </div>
    <div class="col-6">

        <ul>
           <li>16 formas de manos</li>
           <li>800 imagenes</li>
           <li>32x32</li>
           <li>rgb</li>
        </ul>
    </div>
</div>

----

<!-- .slide: style="text-align: left;" -->

## RWTH
<small style="margin-top: -25px;"><em>
Intérpretes de lenguaje de señas en la estación de televisión pública alemana PHOENIX
</em></small>      

<div class="row" style="font-size: 2.53rem;">
    <div class="col-6">
        ![rwth](static/rwth.png)
        <!-- .element: style="width: 75%;" -->
    </div>
    <div class="col-6">
        <ul>
           <li>
                45 formas de manos
                <br>
                <small><em>Nos quedamos con aquellas que cuentan con más de 20 ejemplos.</em></small>
           </li>
           <li>3359 labelled + 17gb unlabeled</li>
           <li>132x92</li>
           <li>rgb</li>
        </ul>
    </div>
</div>

----

<!-- .slide: style="text-align: left;" -->

## CIARP

<div class="row" style="font-size: 2.53rem;">
    <div class="col-6">
        ![ciarp](static/ciarp.png)
        <!-- .element: style="width: 75%;" -->
    </div>
    <div class="col-6">
        <ul>
           <li>10 formas de manos</li>
           <li>6000 imagenes</li>
           <li>38x38</li>
           <li>Cámara de único color</li>
           <li>Etiquetado manual</li>
        </ul>
    </div>
</div>

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

#### Modelos entrenados con diferentes tamaños de muestra

<div class="row" style="width: 125%; transform: translate(-10%, -0%);">
    <div class="col-4">
        ![results](static/results/lsa16.png)
        <strong>LSA16</strong>
    </div>
    <div class="col-4">
        ![results](static/results/rwth.png)
        <strong>RWTH</strong>
    </div>
    <div class="col-4">
        ![results](static/results/ciarp.png)
        <strong>CIARP</strong>
    </div>
</div>

----

# Conclusiones