## Notebooks 2.1 al 2.4.3 — Deep Learning
## Modulo 4: Deep Learning
## Docente: Dr. German Pinedo-Diaz

Estos seis notebooks construyen, de forma progresiva, la arquitectura completa de una red neuronal moderna: desde la unidad más simple hasta el criterio que guía su aprendizaje.

El punto de partida en **2.1** fue entender qué hace realmente una neurona: aplica una transformación afín a la entrada y luego una función de activación (ReLU) que "dobla" el espacio. El resultado es una función lineal a trozos que, bien combinado, puede aproximar casi cualquier cosa.

**2.2** reveló por qué la profundidad importa más que el ancho. Componer redes, pasar la salida de una como entrada de otra, genera exponencialmente más regiones lineales sin aumentar proporcionalmente los parámetros. Dos capas con las mismas neuronas que una sola pueden representar estructuras mucho más complejas. Esta es la justificación matemática detrás del auge de las redes profundas sobre las superficiales.

**2.3** formalizó todo en notación matricial: pesos $\Omega_k$, sesgos $\beta_k$, y el cómputo capa por capa $h_k = \text{ReLU}(\beta_k + \Omega_k h_{k-1})$. Esta representación no es solo matemáticas es la que permite implementar redes eficientemente en hardware y escalar a millones de parámetros.

Los notebooks **2.4.1 al 2.4.3** responden la pregunta más importante: ¿cómo sabe la red si está aprendiendo bien? La respuesta es siempre la misma en su estructura: elegir una distribución para el output, calcular la verosimilitud, tomar su logaritmo y minimizar la pérdida resultante. Regresión usa MSE (Gaussiana), clasificación binaria usa entropía cruzada (Bernoulli + sigmoide), y multiclase añade softmax para obtener probabilidades que sumen uno.

**arquitectura + función de pérdida + optimización** son los tres pilares que definen cualquier red neuronal, sin importar su complejidad.


## Autor Dr. Juan Navarrete Guzman 
TAE Inteligencia Artificial — Modulo 4: Deep Learning CINVESTAV
