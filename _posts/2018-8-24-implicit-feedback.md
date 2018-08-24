---
layout: post
title: Collaborative Filtering for Implicit Feedback Datasets
---

## [Koren, Y., Hu, Y., & Volinsky, C.]

En el paper se describe como los autores implementaron un modelo de filtrado colaborativo que usaba retroalimentación implícita para hacer recomendaciones. Para esto redefinieron la métrica que se usaba en los SVD's normales, usando una suma de los eventos que median. Por otro lado agregaron una métrica de confianza ya que muchos de los valores obtenidos no podían asegurar los gustos de las personas. Al usar distintas técnicas matriciales y ALS para optimizar la factorizacion lograron hacer los cálculos en esta matriz más densa de manera eficiente, por lo que sus resultados se pueden usar en la practica.

En el ejemplo que usaron para testear se uso una métrica para medir gustos, si una persona vió o no algo. Anteriormente habían descrito que existen muchas cosas que se pueden recolectar de manera implícita, con esto surge la pregunta de como se podrían mesclar estos datos para obtener mejores recomendaciones. Este punto no es explorado por los autores pero la combinación de distintas fuentes podría importar para modelos de donde no se pueden obtener muchos datos. Por otro lado tampoco se investiga el uso combinado de ratings explícitos con datos implícitos.

La métrica usada para evaluar el modelo era rank. Hubiera sido bueno si usaran otras métricas para poder decir que su modelo era más completo en distintos aspectos y no solo por un resultado que podrían haber elegido por ser más positivo.
Otra cosa interesante al evaluar sus modelos implícitos es que no lo hayan probado en un dataset con datos explícitos.
Su modelo era mejor que los otros implícitos, pero la diferencia con un modelo explicito importa a la hora de evaluar si valdría la pena recolectar información acerca de los gustos de los usuarios.

Encontré bastante útil que hayan incluido los valores que usaron para sus hiperparametros, ya que a la hora de implementar su modelo es bueno tener una base de donde partir para encontrarlos.

Se describe detalladamente las transformaciones que hicieron para acelerar y escalar los cómputos, por lo que se puede implementar lo que hicieron de manera sencilla. Aunque describen los pasos y su lógica, esta no fue presentada de la mejor manera porque en un párrafo se mezclan muchas ecuaciones distintas y distintos segmentos de esta. Al separarlo en distintas lineas se podría apreciar más intuitivamente lo que logran sin tener que leerlo tantas veces.