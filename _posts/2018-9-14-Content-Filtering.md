---
layout: post
title: Content-based recommendation systems
---

## [Pazzani, M. J., & Billsus, D. (2007)]


El articulo describe distintos métodos de como implementar filtrado basado en contenido.
Para esto comienza explicando como representar distintos ítemes.
Me pareció adecuado que explique como representar datos no estructurados en forma de texto, ya que estos son una de las fuentes más grandes de información. Algo débil en esta descripción fue que se menciono que contando las palabras, sea este tf-idf o bolsas de palabras, se perdía contexto especialmente palabras iguales usadas de manera distinta.
Aunque mencionara esto, no se explica que tan grande es el impacto del problema, o que técnica se ha probado para solucionarlo.
De aquí me surgió la duda si los *word embeddings* como *word to vec* serian útiles en los modelos que describe más adelante.
Otro problema con esta descripción es que no menciona otras fuentes de datos no estructuradas (como imágenes de productos), y esto se nota más adelante cuando en todos los modelos solo afronta el problema de los textos.

Al explicar como se puede aprender un modelo de usuario se menciona que existe impicit y explicit feedback.
Encontré bueno que se mencionaran las ventajas y desventajas de ambos para poder elegir que forma era más útil.
Algo negativo en esto es que no se menciona si los algoritmos descritos después funcionan peor con implicit data, o que al tener mayor volúmenes de información este aporta de manera positiva.

No encontré que las fotos de portales web de perfiles de usuarios haya aportado información al lector.
La mayoría de estos conoce estos portales famosos y se ha visto en frente de un formulario para conocer sus gustos.

En los modelos de *relevance feedback* nos dicen que los algoritmos no aseguran convergencia.
No me quedo claro en que situaciones uno de estos modelos fallaría, o si en la mayoría de los casos funcionan.
Este aspecto seria útil al momento de implementar un modelo, ya que uno podría usar su tiempo y esfuerzo en un modelo con mayor probabilidad de funcionar.

Al hablar de SVM se da una versión muy liviana de como funcionan.
No se menciono si los resultados positivos de los que habla fueron al aplicar kernels para transformar el espacio, o que debido a la gran cantidad de factores estos podían separar lineal mente efectivamente.

Para los algoritmos probabilisticos encontré bueno que explicaran porque los supuestos de independencia no era necesario cumplirlos.
Esto le dio mayor robustez a la explicación de los modelos.

En los últimos párrafos se muestra al lector que aunque el filtrado en base a contenido puede ser usado, este también se puede combinar con otras técnicas para mejorar los resultados.

El paper dio un buen resumen de las principales técnicas y de sus ventajas y desventajas.
Este resumen es bueno para conocer distintas técnica para poder buscar la más apropiada para cada caso.
Aunque dicen que este es un resumen, hubiera sido mejor si sus comentarios hubieran sido explicados con más cifras y métricas, para poder comparar de manera más efectiva que tan bueno es cada modelo.