## Actividades 4 — Optimización en Deep Learning
## Modulo 4: Deep Learning
## Docente: Dr. German Pinedo-Diaz

### 4.1 Descenso por Gradiente
Implementación del descenso por gradiente clásico sobre un modelo lineal simple. Se calcula la función de pérdida de suma de cuadrados, su gradiente analítico y se aplica una búsqueda lineal para elegir el tamaño de paso óptimo en cada iteración. Se visualiza la trayectoria sobre la superficie de pérdida.

### 4.2 Descenso por Gradiente Estocástico (SGD)
Comparación de tres variantes de optimización sobre un modelo Gabor no lineal:
 **SGD con búsqueda lineal**: paso óptimo por iteración.
 **SGD con paso fijo**: tasa de aprendizaje constante. Se experimenta con valores grandes y pequeños de alpha para observar divergencia y convergencia lenta.
 **Mini-batch SGD**: gradiente estimado con un subconjunto aleatorio de datos, introduciendo ruido controlado que permite escapar mínimos locales.
 **Scheduler**: reducción progresiva de alpha por un factor beta cada M iteraciones para afinar la convergencia.

### 4.3 Momentum y Momentum de Nesterov
Implementación de momentum estándar, que acumula una velocidad para suavizar la dirección de actualización, y momentum de Nesterov, que evalúa el gradiente en una posición adelantada. Se comparan las trayectorias de ambos métodos contra SGD estándar sobre la misma superficie de pérdida no convexa.

### 4.4 Adam
Implementación del optimizador Adam, que combina promedios móviles del gradiente y del gradiente cuadrado con corrección de sesgo para adaptar el tamaño de paso por parámetro. Se parte de gradientes normalizados como motivación y se muestra cómo Adam elimina las oscilaciones que estos producen cerca del mínimo.

## Autor
Dr. Juan Navarrete Guzmán
TAE Inteligencia Artificial — Modulo 4: Deep Learning
CINVESTAV
