---
layout: post
title: Factorization Machines
---

## [Steffen Rendle]

En este documento el autor explica las maquinas de factorización.
Para ello las compara con los populares SVM's, para luego mostrar porque son mejores para la recomendación.
Continua explicando como se hacen predicciones y se entrenan, para finalmente compararlas con los modelos populares del momento.

Encuentro que la comparación con los SVM's en el comienzo ayuda a hacerse una intuición inmediata de porque se crearon los maquinas de factorización.
También ayudan a entender el concepto que se quiere obtener, una forma de hacer predicciones con *kernels* distintos.
Por otro lado, asume que el lector tiene un conocimiento de SVM, lo cual puede no ser el caso.
Esto haría más complejo a introducción que justo buscaba hacer lo contrario con la comparación.

En el sector de expresividad se menciona que es conocido la factorización de una matriz positiva definida en V con un k elevado.
Yo no conocía esta factorización y el paper no dio un vinculo a alguno que lo explique.
Sin embargo, incluso sin conocer la descomposición se entiende porque al disminuir k se puede obtener mayor generalización; se hace menos *overfitting*.

Al explicar que se puede usar descenso del gradiente para aprender los parámetros, no se detalla bien como se haría su aplicación.
Uno sabe que se deben ir actualizando los valores en cada iteración, pero no se explica como exactamente se hace para los distintos parámetros.
Me pareció que este punto, que es una ventaja de los FM al poder aplicarlos a varias funciones de perdida, podría haber sido expandido.

El siguiente sector, donde compara los distinto modelos contra el FM, lo encontré muy útil a la hora de ver las ventajas del este modelo.
En la parte anterior el autor menciono que se podían modelar todos ellos con una FM y en esta se da la evidencia.
Por otro lado también se muestra que es relativamente sencillo aplicar una FM para estos modelos, lo que convence más que estas son una técnica importante.

En resumen, el autor es capaz de mostrar como funcionan las FM y de dar ejemplos de como pueden sustituir los modelos más populares actuales.
Aunque esto lo logra de buena manera, la complejidad de las matemáticas y la falta de algunas explicaciones básicas hacen que el paper no sea tan fácil de seguir.