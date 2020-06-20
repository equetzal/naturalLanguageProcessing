
# Clase Online #1

**Fecha:** 20.marzo.2020

## Actividad Online 1

Ver los videos de las clases impartidas por [Andrew Ng](https://es.wikipedia.org/wiki/Andrew_Ng)

Los videos están [en esta lista](https://www.youtube.com/playlist?list=PLLssT5z_DsK-h9vYZkQkYNWcItqhlRJLN).
 
Por favor, hasta mañana estudian [Lecture 1.1](https://youtu.be/PPLop4L2eGk), [Lecture 1.2](https://youtu.be/bQI5uDxrFfA), [Lecture 1.3](https://youtu.be/jAA2g9ItoAc)


## Teoría

*¿Cómo la máquina aprende?*

Le damos datos, también se llaman ejemplos. Cada ejemplo es un vector numérico que representa el dato correspondiente. Para imágenes, el vector va a contener los valores de intensidades de colores de pixeles, para nosotros son características que estudiamos: frecuencia bruta, frecuencia relativa (probabilidad), tf-idf, etc. de palabras. 

Los vectores de ejemplos se representan como $x^{(i)}$ donde $i$ es el número del ejemplo. Los elementos (features) del vector también se representan por $x$, pero por $x$ con subíndice, por ejemplo, $x_j$ donde $j$ es el número del elemento del vector.

Entonces cada dato es el vector de este tipo:
$x^{(i)} = (x_1, x_2, \dots, x_j, \dots, x_n)$, para toda $1\leq j \leq n$

$m$ es el número de ejemplos y $n$ es el número de características en un vector (longitud del vector).

Cada vector $x^{(i)}$, está asociado con un valor que se representa por $y^{(i)}$. Entonces el conjunto de datos del tamaño $m$, va a contener los pares de tipo $(x^{(i)},y^{(i)})$.

La idea de aprendizaje es enseñar a la máquina estos ejemplos (pares de tipo $(x^{(i)},y^{(i)})$, para que halla aprenda a predecir el valor de $y^{(i)}$ a partir del vector $x^{(i)}$.

*¿Como precisamente se realiza este aprendizaje?*

La máquina toma un vector $x^{(i)}$ y calcula el valor de $y$ que le corresponde a $x^{(i)}$ usando una cierta función o proceso. Este valor calculado de $y$ se llama el valor estimado de $y$, y se
representa por $\hat{y}^{(i)}$. Este valor $\hat{y}^{(i)}$ normalmente es diferente del valor real $y^{(i)}$, es decir, hay un error de estimación. El error se puede calcular usando el método de diferencias cuadradas:
$$
errorDeEstimación = (\hat{y}^{(i)}-y^{(i)})^2
$$

El error de estimación o predicción también se llama **costo**. Para cada ejemplo se calcula el error
de predicción, luego se suman todos los errores y se promedian por el número 𝑚 de ejemplos.
Este promedio se llama **función de costo** que se denomina por la letra $J$
$$
J = \dfrac{1}{2m}\sum_{i=1}^{m}(\hat{y}^{(i)}-y^{(i)})^2
$$

La función de costo a veces se llama función de pérdida o función de error.
Ahora lo que hay que hacer es optimizar la función de costo, es decir, minimizar el error de predicción. El proceso de optimización se llama aprendizaje.

## Actividad Online 2
Por favor vean los videos:
- [Lecture 2.1](https://youtu.be/kHwlB_j7Hkc)
- [Lecture 2.2](https://youtu.be/yuH4iRcggMw) 
- [Lecture 2.3](https://youtu.be/yR2ipCoFvNo)
- [Lecture 2.4](https://youtu.be/0kns1gXLYg4)

Estudien bien su contenido, en estas clases ustedes van a conocer como se calcula el valor estimado de $\hat{y}^{(i)}$
