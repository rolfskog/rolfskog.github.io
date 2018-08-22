---
layout: post
title: Matrix Facorization Techniques for Recommender Systems
---

## [Koren, Y., Bell, R., & Volinsky, C.]

En este paper, los autores describen los beneficios de usar técnicas de factorización de matrices para sistemas recomendadores. Para hacer esto primero describen las solución general al problema, planteando la función de perdida y como se soluciona. Luego exploran distintos aspectos que se pueden incorporar para mejorar la exacitud de los sistemas, como la incorporación de retroalimentación implícita. Por ultimo muestran como sus técnicas mejoraron los resultados en el netflix prize.

Los autores muestran como se pueden agregar distintos factores a la ecuación para poder tomar en consideración cosas como sesgos. Encuentro útil que hayan decidido incluir como estos se podrían agregar, incluyéndose en a perdida y como factores de regularización. Por otro lado se ignora como al agregar mas términos se haría mas ineficiente la optimización. Esta discusión es importante ya que se esta proponiendo que son mas eficientes en tiempo y recursos que otros modelos, por lo que al hacerlos mas complejos importa el aumento de complejidad en ejecución.

Cuando se explica la implementación con gradient descent, se muestra mediante ecuaciones como se actualizan los términos. Para ALS se describe que se mantiene una constante y que por eso se puede paralelizar. No me queda tan claro como se implementaría, especialmente como se elije esa constante y que tipo de optimización de hace. Tampoco se explica como cambia el algoritmo al ir agregando mas factores y si los beneficios de ALS siguen siendo iguales o la diferencia es mayor al poder paralelizarse más.