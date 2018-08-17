---
layout: post
title: Collaborative filtering recommender systems
---

## [Schafer, J. B., Frankowski, D., Herlocker, J., & Sen, S. (2007)]

El paper intenta hacer un resumen del estado del arte para sistemas de filtrado colaborativo.
Para esto explica como surgió la idea de filtrado colaborativo, como funcionan y para que sirven.
Luego describe formas típicas de implementaros y problemas y desafíos relacionados con su creación e implementacion.
Termina presentando distintas formas de evaluar los recomendadores y de desafíos que todavía no tenían solución.

### Discusión

#### Positivos

* Cuando los autores describen un nuevo algoritmo (como user based y item based), ellos comienzan con describir la intuición detrás de ellos. Esto ayuda a que los lectores entiendan lo que esta sucediendo antes de desarrollar las formulas matemáticas, lo que no pasa siempre en papers científicos.

* Me parece interesante que decidieron explicar las métricas mas utilizadas en profundidad (Accuracy y precision), para luego mostrar que existen muchas otras métricas normalmente dejadas de lado pero que pueden tener un impacto importante en como se perciben los sistemas.

#### Negativos

* Se entregan y comparan muchos distintos algoritmos y modelos para hacer recomendaciones. Estas comparaciones son echas mediante intuiciones acerca de porque en distintos dominios algunos recomendadores son mas útiles. El problema es que no se entrega mucha evidencia para corroborar estas intuiciones, como resultados de distintos experimentos. Lo único que hacen los autores es linkear a oros papers, sin describir lo que se encuentra en ellos.

* En el paper se menciona que los usuarios que participan del proceso de recomendacion (por ejemplo bloqueando otros individuos) sacan mas provecho de los sitios. Me quedo la duda al leer esto de porque esto podría beneficiar a los usuarios, ya que la cantidad de input de un usuario no se podría acercar a la cantidad recolectada explícitamente e implícitamente. El paper profundiza en las consecuencias para los modelos que siguen estos pasos.
