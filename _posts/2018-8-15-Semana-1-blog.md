---
layout: post
title: How not to sort by Average Rating
---

## [Evan Miller Blog](http://www.evanmiller.org/how-not-to-sort-by-average-rating.html)

El blog explora distintas formas de calcular scores, presentandonos primero average rating y (Positive ratings) − (Negative ratings) para luego explicar porque el score calculado mediante el lower bound of Wilson score es mejor.

### Discusión

#### Positivos

* La forma de presentar la información es sencilla de digerir, nos presenta una forma de calcular score, da argumentos de porque esta es negativa y luego presenta une ejemplo de un sistema que lo ocupa.

* Describe detalladamente que es el Wilson score y que significa el intervalo de confianza que se elige al construir el puntaje. Con esto explica que este score es mas adecuado ya que toma en consideración la incertidumbre en la respuesta. También se dan distintas formas de implementar el método lo que ayuda al lector ya que se ve que se puede implementar con unas pocas lineas de código.

#### Negativos

* El blog no describe como usar el Wilson score cuando tenemos ratings calcados de manera distinta, por ejemplo con estrellas. Esto significa que no explora las distintas implicancias de ir variando el umbral de corte y como afectaría los rankings. Esto tambien es importante para el blog ya que uno de los ejemplos provistos usa un formato de ratings con estrellas, lo cual hace que pareciera que no satisfaga tanto su punto.

* El autor desea convencer al lector que las primeras dos soluciones son malas y no debiesen ser ocupadas. Esto lleva a que no especifica en que ocasiones estas formas de calcular el score son mejores o alguien desearía implementarlas. Hubiera sido interesante conocer los pros ademas del contra de esas opciones para poder convencer de manera mas competa y cuando el Wilson score es mejor. 
