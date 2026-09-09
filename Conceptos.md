# Definición de conceptos
Se describirán los conceptos sobre estadistica básica.

## Tabla de contenidos
- Frecuencia de elementos
- Media estadistica de elementos
- Desviación estandar
- Mínimo
- Percentiles
- Máximo

### Frecuencia de elementos
La función count() de Python se ocupa para obtener la ocurrencia de los elementos de una lista de cadenas o tuplas

  - string.count(substring, start, end) -> para cadenas de texto
  - count = numbers.count(2) -> para lista de elementos

### Media estadistica de elementos
La función statistics.mean() de Python se ocupa para obtener la media de una serie de elementos 

  - Librería numpy para la media -> numpy.mean()
  - Librería pandas para la media -> df.mean()

### Desviación estandar
La función statistics.stdev() de Python se ocupa para obtener la desviación estandar de una serie de elementos 

  - Librería numpy para la desviación estándar -> np.std() -> Recomendado para vectores y matrices
  - Librería pandas para la desviación estándar -> df[----].std() -> Recomendado para DataFrames y CSV's


### Minimo
La función min() de Python se ocupa para obtener el elemento de mínimo valor de los elementos de una lista, cadenas o tuplas

  - print(min(words)) -> para cadenas de texto
  - min(iterable, *[, key, default]), min(arg1, arg2, *args[, key]) -> funciones avanzadas con llaves complejas
    
### Percentiles
La función 25%(), 50%(), 75%() de Python se ocupan para obtener las porcentajes de una serie de elementos 

 ### Maximo
La función max() de Python se ocupa para obtener el elemento de mínimo valor de los elementos de una lista, cadenas o tuplas

  
