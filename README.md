# Laboratorio 1

## Problema 1

Dado un arreglo de números `A`, de largo `N` y un número
entero `K`, se debe encontrar el máximo entero para cada
sub-arreglo contiguo de largo `K` que se puede formar en
orden a partir de `A`.

Por ejemplo, si `A` es `[2,3,4,5,6,2,3]` y `K` es igual a 3.
Los sub-arreglos contiguos en orden que se pueden formar a partir
de `A` son: `[2,3,4]`, `[3,4,5]`, `[4,5,6]`, `[5,6,2]`,
`[6,2,3]`. Lo que se pide encontrar son los máximos de cada
uno de estos sub-arreglos, en este caso corresponden a:

- `[2,3,4]` el máximo es `4`
- `[3,4,5]` el máximo es `5`
- `[4,5,6]` el máximo es `6`
- `[5,6,2]` el máximo es `6`

### Formato de entrada

La primera línea de entrada contendrá un número `T` que corresponde
al número de casos de prueba. Cada caso de prueba estará compuesto
de dos líneas:

- La primera línea contendrá dos números `N` y `K` separados por
  un espacio, donde `N` representa el largo del arreglo `A` para
  este caso de prueba y `K` representa en largo de los
  sub-arreglos a formar.
- La segunda línea contendrá los elementos de `A` separados por
  espacios.

### Restricciones

1 ≤ `T` ≤ 1000

1 ≤ `N` ≤ 10000

1 ≤ `K` ≤ `N`

1 ≤ `A`<sub>i</sub> ≤ 10000, donde `A`<sub>i</sub> es el i-ésimo
elemento en el arreglo `A`.

### Formato de salida

Por cada caso de prueba imprimir una sola línea que contenga los
máximos de cada sub-arreglo separados por un espacio.

### Ejemplo

#### Entrada

```
2
5 2
3 4 6 3 4
7 4
3 4 5 8 1 4 10
```

#### Salida

```
4 6 6 4
8 8 8 10
```

#### Explicación

Para el primer caso, los sub-arreglos de largo 2 q se pueden formar
son `[3,4]`, `[4,6]`, `[6,3]` y `[3,4]`, donde los máximos de cada
uno de éstos corresponden a `4 6 6 4`.

Para el segundo caso los sub-arreglos de largo 4 que se pueden formar
son `[3,4,5,8]`, `[4,5,8,1]`, `[5,8,1,4]` y `[8,1,4,10]`, donde los
máximos de cada uno de éstos corresponden a `8 8 8 10`.


## Problema 2

Un histograma es un polígono compuesto por una secuencia de
**react**ángulos alineados por una línea base comun. Los
**react**ángulos tienen el mismo ancho pero diferentes alturas.
Por ejemplo, en la siguiente figura es mostrado un histograma
compuesto por **react**ángulos de alturas 2, 1, 4, 5, 1, 3, 3,
medido en unidades donde 1 es el ancho de los **react**ángulos.

![histogram](http://www.informatik.uni-ulm.de/acm/Locals/2003/html/images/histogram.gif)

Para este problema se le pide calcular el área del **react**ángulo
más grande presente en un histograma que este alineado con la línea
base. La figura a la derecha muestra el **react**ángulo más grande
presente en ese histograma.

### Formato de entrada

La primera línea contine solo un número entero `N` que representa
el número de **react**ángulos en el histograma.
La segundo línea contiene `N` números enteros `h`<sub>i</sub>
separados por espacios, representado las alturas de cada uno de
los **react**angulos en el histograma.

### Restricciones

1 ≤ `N` ≤ 10<sup>5</sup>

1 ≤ `h`<sub>i</sub> ≤ 10<sup>6</sup>

## Formato de salida

Debe imprimir un solo número entero representado el área del
**react**ángulo más grande que se puede formar en el histograma
dado.

## Ejemplo

### Entrada

```
25
5 4 3 2 1 2 3 4 5 1 1 5 5 5 1 1 5 5 5 1 3 1 5 5 5
```

### Salida

```
25
```

### Explicacíon

Las alturas dadas `1 2 3 4 5`, forman el siguiente histograma:

```
•       •  •••  •••   •••
••     ••  •••  •••   •••
•••   •••  •••  ••• • •••
•••• ••••  •••  ••• • •••
•••••••••••••••••••••••••
```

El **react**ángulo más grande o con el área máxima es el siguiente.

```
•       •  •••  •••   •••
••     ••  •••  •••   •••
•••   •••  •••  ••• • •••
•••• ••••  •••  ••• • •••
xxxxxxxxxxxxxxxxxxxxxxxxx
```
