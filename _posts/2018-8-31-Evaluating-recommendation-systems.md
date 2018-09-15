---
layout: post
title: Evaluating recommendation systems
---

## [Shani, Guy, and Asela Gunawardana]

Este capitulo del libro busca explicar las principales manera de evaluar un sistema recomendador. Para esto separa las formas de evaluar en tres zona, pruebas offline, estudios de usuarios y pruebas online.
Luego describe distintas evaluaciones para las cuales uno estaría interesado.
Al explorar varias formas distintas de evaluar se busca que los lectores se den cuenta que los distintos sistemas pueden ser mejores para distintas tareas, por lo que se debe saber el propósito del sistema para mejor la experiencia del usuario.
Ademas de entregar las métricas normales para evaluar, se presentan distintos problemas asociados, por ejemplo escalabilidad y privacidad.

Durante la explicación de test de hipótesis, los autores mencionan varias pruebas distintas que contienen distintos supuestos de normalidad y de independencia.
Se asume que el lector conoce como identificar si estos supuestos se cumplen en su datasets, como para que se cumplan los supuestos del t-student, para poder validar que la prueba haga sentido.
Hubiera sido útil un párrafo explicando esto o un vinculo a algún trabajo que lo haga como hicieron para ANOVA.
Tampoco mencionan algún ejemplo de investigación donde se ocuparan las pruebas en sistemas recomendadores.

En la sección de utility ranking, se mencionan tres estadísticos comúnmente usados.
Me surgió la duda de porque decidieron no mencionar otros estadísticos comunes como MAP o average rank, los cuales aparecen comúnmente en papers sobre recomendación.
Esto va de la mano con que en online test se describe una forma de hacer mediciones, pero no se presenta una formula o nombre matemático para implementarlo, lo que dificulta el entendimiento y comparación con los modelos offline.

Me aparece adecuado que para cada explicación de como medir el rendimiento se pongan los casos de offline y online tests.
De esta manera se puede implementar de manera mas sencilla y al mismo tiempo comparar las dificultades y beneficios de hacer distintas pruebas con usuarios reales.

La descripción sobre la confianza de las predicciones era confusa, ya que se describía un problema matemático usando palabras.
Esto se corrigió entregando un ejemplo bien elaborado con una métrica estándar de confianza.
Dar un ejemplo así para un concepto intuitivamente confuso ayudo a que la lectura sea mas fluida, al no tener que releer un párrafo específico.
Esto se ve replicado en explicaciones posteriores, facilitando el entendimiento

Se explica una nueva forma de evaluar un sistema usando un intervalo de confianza, pero luego se dice que no hay una forma clara de deducir como esto mejora la experiencia de usuario.
Esto hace parecer que esta técnica no es muy adecuada, por lo que no agrega valor al paper sin mayor explicación de porque seria ventajoso usarla.

En conclusión, este articulo explica distintos aspectos importantes que cualquier persona interesada en sistemas recomendadores debería considerar al momento de evaluar sus sistema.
Aunque las descripciones son buenas, estas persiguen explicar conceptos, dejando de lado la implementación por lo que un lector interesado tendría que investigar mas para poder usar lo aprendido en la practica.