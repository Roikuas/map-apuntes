<!-- Módulo statistics  python -->
# Mapa Mental del Módulo `statistics` en Python

## Introducción
- El módulo `statistics` proporciona funciones para realizar estadísticas matemáticas sobre datos numéricos reales.

## Tipos de Datos Aceptados
- **Listas**
- **Tuplas**
- **Iteradores**

## Funciones Descriptivas

### Medidas de Tendencia Central
- **mean(data)**
  - Calcula la media aritmética de los datos.
- **median(data)**
  - Calcula la mediana (valor medio) de los datos.
- **mode(data)**
  - Encuentra el valor más común (moda) en los datos.
- **median_low(data)**
  - Retorna la mediana de los datos cuando el número de elementos es impar.
- **median_high(data)**
  - Retorna la mediana de los datos cuando el número de elementos es impar.
- **median_grouped(data, interval=1)**
  - Calcula la mediana de datos agrupados.

### Medidas de Dispersión
- **pstdev(data, mu=None)**
  - Calcula la desviación estándar de la población.
- **pvariance(data, mu=None)**
  - Calcula la varianza de la población.
- **stdev(data, xbar=None)**
  - Calcula la desviación estándar de la muestra.
- **variance(data, xbar=None)**
  - Calcula la varianza de la muestra.

### Medidas de Posición
- **quantiles(data, n=4, method='exclusive')**
  - Divide los datos en intervalos iguales.
  - **n**: Número de intervalos.
  - **method**: Método para el cálculo de cuantiles (`'exclusive'` o `'inclusive'`).

## Funciones de Estadísticas Robusta
- **fmean(data)**
  - Calcula la media aritmética de los datos, mejorada para números flotantes.
- **geometric_mean(data)**
  - Calcula la media geométrica de los datos.
- **harmonic_mean(data)**
  - Calcula la media armónica de los datos.
- **multimode(data)**
  - Encuentra todas las modas en los datos.

## Otras Funciones
- **StatisticsError**
  - Clase de excepción para errores específicos de estadísticas.
  
## Ejemplos de Uso

### Media Aritmética
```python
import statistics as stats
data = [1, 2, 3, 4, 5]
print(stats.mean(data))
```
### Mediana 
```python
import statistics as stats
data = [1, 2, 3, 4, 5]
print(stats.median(data))
```
### Moda 
```python
import statistics as stats
data = [1, 1, 2, 3, 4]
print(stats.mode(data))
```
### Desviación Estandar de la Muestra 
```python
import statistics as stats
data = [1, 2, 3, 4, 5]
print(stats.stdev(data))
```
### Cuantiles 
```python
import statistics as stats
data = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
print(stats.quantiles(data, n=4))

```












