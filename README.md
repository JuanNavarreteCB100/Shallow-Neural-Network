# Math Warm-Up — TAE Inteligencia Artificial
## Modulo 4: Deep Learning
# Docente: German Pinedo-Diaz

Las actividades estan dividias por secciones:

# Actividades 1: 

1.1 — Math Warm-Up

Funciones lineales y afines — diferencia entre g(x) = ωx (lineal pura) y f(x) = β + ωx (afín), y por qué en DL se les llama coloquialmente "lineales".
Funciones no lineales — motivación para usar activaciones (ReLU, sigmoid, tanh): apilar capas puramente lineales sigue siendo lineal, las no linealidades crean las "curvas" que permiten modelar patrones complejos.
Derivadas y gradientes — interpretación intuitiva como "brújula" de aprendizaje; el gradiente indica la dirección para ajustar parámetros y reducir la pérdida.
Ejercicios prácticos — implementación de funciones lineales en NumPy con pruebas unitarias, visualización de campos de gradiente en 2D con matplotlib.

1.2 — Regresión Lineal 1D

Modelo lineal — implementación de f(x, φ₀, φ₁) = φ₀ + φ₁·x con intercept y pendiente.
Función de pérdida — cálculo del error cuadrático (ecuación 2.5) para evaluar qué tan bien ajusta el modelo.
Optimización manual — ajuste coordenada por coordenada de φ₀ y φ₁ para minimizar la pérdida (descenso de coordenadas).
Visualización del espacio de pérdida — mapa de calor y curvas de nivel en 2D para comprender la superficie de optimización.

# Actividades 2

2.1 — Redes Neuronales Superficiales (Shallow Neural Networks)_ Construcción e interpretación de redes de una sola capa oculta:

Activación ReLU — implementación y visualización de la función de activación rectificada.
Red 1-entrada / 3-neuronas / 1-salida — cálculo manual de preactivaciones, activaciones y salida final con parámetros θ y φ.
Regiones lineales — análisis de cuántos politopos lineales genera el modelo (7 regiones con 3 unidades ReLU en 2D).
Ajuste a datos — uso de la pérdida de mínimos cuadrados para entrenar la red; exploración del espacio de parámetros.
Múltiples salidas — extensión a dos salidas visualizadas con mapas de calor separados.

2.2 — Composición de Redes Neuronales_ Apilamiento de dos redes independientes como bloque modular:

Composición funcional — la salida de la red 1 se alimenta como entrada a la red 2, construyendo representaciones más ricas.
Visualización end-to-end — trazado de la función compuesta en el rango [-1, 1].

2.3 — Redes Neuronales Profundas (Deep Neural Networks)_ Extensión a múltiples capas ocultas usando álgebra matricial:

Formulación matricial — reimplementación de la red usando multiplicaciones de matrices (ecuación 4.15).
Red profunda 3 capas — arquitectura 4→5→2→4→1; propagación hacia adelante completa.
Concatenación de redes — alimentar la salida de una red como entrada de otra para construir profundidad.

2.4.1 — Función de Pérdida I: Regresión Univariada
Análisis de criterios de optimización para regresión:

Likelihood y log-likelihood negativa — cálculo e interpretación; comparación con mínimos cuadrados.
Distribución gaussiana — efecto de μ y σ sobre el ajuste del modelo.
Descenso por coordenadas — variación de un parámetro a la vez (beta_1, sigma) para observar la superficie de pérdida.

2.4.2 — Función de Pérdida II: Clasificación Binaria
Criterios de optimización para clasificación de dos clases:

Función sigmoide — transformación de la salida de la red al rango [0, 1] para representar probabilidades.
Binary cross-entropy — cálculo de likelihood y log-likelihood negativa para datos binarios.
Análisis de parámetros — efecto de beta_1 sobre ambas métricas; motivación práctica de la log-likelihood.

2.4.3 — Tarea: Función de Pérdida III: Clasificación Multiclase
Extensión a K clases con softmax y entropía cruzada:

Función softmax — normalización de K salidas arbitrarias a probabilidades válidas (no negativas, suma 1).
Multiclass cross-entropy — likelihood y log-likelihood negativa para 3 clases (rojo, verde, azul).
Optimización de red completa — exploración de los 16 parámetros β₀, Ω₀, β₁, Ω₁ que minimizan la pérdida.

# Actividades 3


# Actividades 4 


## Autor
#Dr. Juan Navarrete Guzman
#TAE Inteligencia Artificial — Modulo 4: Deep Learning
#CINVESTAV
