# Breve repaso por las matemáticas en que se basa

Para adentrarnos en el mundo del Machine Learning, deberemos viajar a través de una gran cantidad de matemáticas.

En primer lugar, las matemáticas serán necesarias para seleccionar el algoritmo correcto, teniendo en cuenta la precisión requerida, el tiempo necesario, la complejidad del modelo, el número de parámetros de entrada y demás características. Elegir el algoritmo correcto se convierte pues, en un problema matemático de optimización.

También para seleccionar parámetros y estrategias de validación, así como para realizar ajustes y estimar el invervalo de confianza y la incertidumbre.

## Álgebra lineal

Lo primero que nos encontraremos al tratar problemas de Machine Learning es álgebra lineal, ya que es prácticamente omnipresente a lo largo y ancho del proceso: transformación de coordenadas, reducción de dimensionalidad, regresión lineal, solución de sistemas lineales de ecuaciones, etc.

El álgebra lineal es la rama de las matemáticas que estudia los espacios vectoriales y las transformaciones lineales, que son funciones entre espacios vectoriales que satisfacen:

$$T(u+v)=T(u)+T(v)$$
$$T(r·v)=r·T(v)$$

Los espacios vectoriales más comunes toman valores enteros o reales. Se suele trabajar en el conjunto $R^n$, por lo que lo habitual es trabajar con matrices $m\times n$.

El álgebra lineal tiene, además, múltiples conexiones con otras ramas de las matemáticas que influyen en el Machine Learning, como el análisis funcional, las ecuaciones diferenciales, la investigación de operaciones, etc.

## Probabilidad y estadística

El Machine Learning se basa fundamentalmente en resultados estadísticos. La Probabilidad proporciona el marco para representar y cuantificar la incertidumbre, así como axiomas para deducir nuevos estados de incertidumbre.

Los conceptos de probabilidad y estadística que podemos destacar como más importantes en el Machine Learning son la combinatoria, las reglas de probabilidad, el Teorema de Bayes, variables aleatorias, varianza, distribuciones condicionales y conjuntas, distribuciones estándar (Bernoulli, Binomial, Multinomial, Uniforme, Gaussiana,...), estimación de máxima verosimilitud, estimación máxima a posteriori, métodos de muestreo, etc.

## Cálculo vectorial

El Machine Learning implementa, también, resultados del cálculo vectorial, que es una generalización a varias variables del cálculo infinitesimal e integral.

Además del cálculo diferencial e integral, se utilizan derivadas parciales, funciones de valores vectoriales, gradiente direccional, matriz Hessiana, Jacobiano, Laplaciano y función lagrangiana.

## Cálculo numérico

Actualmente las librerías de código que se utilizan, implementan diversos métodos de análisis numérico.

Hay dos problemas fundamentales relacionados con esta disciplina: por una parte, la enorme cantidad de datos con los que se trabaja, supone un elevado coste computacional tanto en memoria, como en procesamiento a la hora de realizar cálculos.

Por otra parte, la capacidad finita de las máquinas, que implica trabajar con un número finito de decimales, lo cual supone introducir un error por aproximación (truncamiento o redondeo). Ese error, puede aumentar exponencialmente si no se tiene en cuenta a la hora de implementarlo en nuestros algoritmos. Además, algunos sistemas son inestables y una diferencia mínima de los datos, produce diferencias enormes en los resultados. Es lo que se conoce como Efecto Mariposa, y es la principal dificultad, por ejemplo, de la predicción del tiempo en un plazo superior a 4 días.