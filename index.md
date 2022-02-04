---
layout: default
---
# Portfolio

## Dereverberación del habla utilizando Redes Neuronales Convolucionales (CNN)

En este trabajo se estudia la dereverberación de señales de habla a partir de algoritmos de aprendizaje profundo. Se implementa una red neuronal convolucional tipo autoencoder con conexiones de salto, basada en el estado del arte actual, para estimar máscaras de amplitud que realicen la dereverberación del habla en el dominio de la transformada de tiempo corto de Fourier. Uno de los problemas de esta tarea es la escasa cantidad de datos disponibles, por lo que se analizan técnicas de generación y aumentación de datos, evaluando su impacto en el desempeño del sistema. Además, se evalúa el efecto que tiene el ordenamiento de los datos de entrenamiento y el tratamiento de la información de fase. 

![Estructura Implementada](/images/modelo_red.png)

Los resultados indican que las técnicas de generación y aumentación de datos permiten mejorar el rendimiento final del sistema. A su vez, ordenar los datos de entrenamiento con un tiempo de reverberación creciente tuvo un impacto positivo en las métricas de evaluación. Por último, se proponen mejoras al enfoque utilizado, y líneas futuras de investigación.

Este trabajo corresponde a la tesis realizada para optar por el titulo de Ingeniero de Sonido en la Universidad Nacional de Tres de Febrero (Untref), y fue presentado en noviembre de 2021. El documento completo esta disponible en este <a href="pdf/Meza_Dereverberación del habla a partir de algoritmos de aprendizaje profundo.pdf">link</a>.

<p align="center">
<a href="https://martinbmeza.github.io/deep-dereverb/">Seguir leyendo</a> |
<a href="https://github.com/martinBmeza/deep-dereverb">Ver repositorio</a>
</p>


## Análisis y Aumentación de Respuestas al Impulso

Las bases de datos de respuestas al impulso reales generalmente son pocas y no logran una buena cobertura de los parámetros acústicos como el T60 y el DRR. Es posible, mediante técnicas de procesamiento de señales, alterar los parámetros acústicos de una respuesta al impulso, generando otras con distintas características acústicas. De esta forma, se puede ampliar considerablemente la cantidad de respuestas al impulso del conjunto de datos, a partir de alteraciones a un conjunto pequeño de respuestas al impulso reales, logrando una mejor cobertura de los parámetros acústicos de interés. En este trabajo, se utilizan dos procesos para aumentar las respuestas al impulso reales: una alteración de amplitud en la parte temprana de la respuesta al impulso para controlar la relación directo-reverberado, y una alteración de envolvente de caída para controlar el tiempo de reverberación.

![Aumentacion](/images/tr_aug.png)

Ademas, en este proyecto, se incluyen herramientas de código en Python para el análisis acústico de respuestas al impulso, como filtrado, calculo del tiempo de reverberación por bandas, cálculo de la relación directo reverberado, e implementaciones de métodos de estimación de piso de ruido. Estas son herramientas siempre útiles para trabajar en procesos que requieran analizar respuestas al impulso. 

![Filtros](/images/banco_filtros.png)

<p align="center">
<a href="pdf/rir_aug.pdf">Seguir leyendo</a> |
<a href="https://github.com/martinBmeza/rir_analysis">Ver repositorio</a>
</p>

# Plantilla
Text can be **bold**, _italic_, or ~~strikethrough~~.

[Link to another page](./another-page.html).

There should be whitespace between paragraphs.

There should be whitespace between paragraphs. We recommend including a README, or a file with information about your project.

# Header 1

This is a normal paragraph following a header. GitHub is a code hosting platform for version control and collaboration. It lets you and others work together on projects from anywhere.

## Header 2

> This is a blockquote following a header.
>
> When something is important enough, you do it even if the odds are not in your favor.

### Header 3

```js
// Javascript code with syntax highlighting.
var fun = function lang(l) {
  dateformat.i18n = require('./lang/' + l)
  return true;
}
```

```ruby
# Ruby code with syntax highlighting
GitHubPages::Dependencies.gems.each do |gem, version|
  s.add_dependency(gem, "= #{version}")
end
```

#### Header 4

*   This is an unordered list following a header.
*   This is an unordered list following a header.
*   This is an unordered list following a header.

##### Header 5

1.  This is an ordered list following a header.
2.  This is an ordered list following a header.
3.  This is an ordered list following a header.

###### Header 6

| head1        | head two          | three |
|:-------------|:------------------|:------|
| ok           | good swedish fish | nice  |
| out of stock | good and plenty   | nice  |
| ok           | good `oreos`      | hmm   |
| ok           | good `zoute` drop | yumm  |

### There's a horizontal rule below this.

* * *

### Here is an unordered list:

*   Item foo
*   Item bar
*   Item baz
*   Item zip

### And an ordered list:

1.  Item one
1.  Item two
1.  Item three
1.  Item four

### And a nested list:

- level 1 item
  - level 2 item
  - level 2 item
    - level 3 item
    - level 3 item
- level 1 item
  - level 2 item
  - level 2 item
  - level 2 item
- level 1 item
  - level 2 item
  - level 2 item
- level 1 item

### Small image

![Octocat](https://github.githubassets.com/images/icons/emoji/octocat.png)

### Large image

![Branching](https://guides.github.com/activities/hello-world/branching.png)


### Definition lists can be used with HTML syntax.

<dl>
<dt>Name</dt>
<dd>Godzilla</dd>
<dt>Born</dt>
<dd>1952</dd>
<dt>Birthplace</dt>
<dd>Japan</dd>
<dt>Color</dt>
<dd>Green</dd>
</dl>

```
Long, single-line code blocks should not wrap. They should horizontally scroll if they are too long. This line should be long enough to demonstrate this.
```

```
The final element.
```
