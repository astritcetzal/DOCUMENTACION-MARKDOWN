# Documentación de ejercicios- Astrit 
## Tecnológico de Software
## *Materia:* Fundamentos de álgebra
## *Fecha:* 18/11/2025
## *Alumno:* Astrit Airan Cetzal Cetzal
## *Actividad* \#18 - Matrices doc
## *Grupo:* C
## El objetivo de esta actividad es resolver problemas que implican matrices, buscando la determinante, utilizando el método de Sarrus, el de cofactores, al igual que la verificacion de propiedades y la aplicación de la determinante en geometria.
## Ejercicios realizados 

### Ejercicio 1: Determinantes 2 x 2

$$ A =
\begin{pmatrix}
5 & 2 \\
3 & 1 \\
\end{pmatrix}
$$

#### *Paso 1: Multiplicar diagonales*
#### 5 x 1= 5   |   -1(2 x 3)= -6
#### *Paso 2: Sumar el resultado de las multiplicaciones*
#### 5 - 6 = -1
#### *Resultado:* det(A)= -1

$$ B =
\begin{pmatrix}
-1 & 4 \\
2 & -8 \\
\end{pmatrix}
$$

#### *Paso 1: Multiplicar diagonales*
#### -(2 x 4)= -8   |   (-1 x -8)= 8
#### *Paso 2: Sumar el resultado de las multiplicaciones*
#### 8 - 8 = 0
#### *Resultado:* det(B)= 0

$$ C =
\begin{pmatrix}
6 & 9 \\
2 & 3 \\
\end{pmatrix}
$$

#### *Paso 1: Multiplicar diagonales*
#### 6 x 3= 18   |   -(2x 9)= -8
#### *Paso 2: Sumar el resultado de las multiplicaciones*
#### 18 - 18 = 0
#### *Resultado:* det(C)= 0

$$ D =
\begin{pmatrix}
0 & 5 \\
-5 & 0 \\
\end{pmatrix}
$$

#### *Paso 1: Multiplicar diagonales*
#### 0 x 0= 0   |   -(5 x -5)= 25
#### *Paso 2: Sumar el resultado de las multiplicaciones*
#### 25 - 0 = 25
#### *Resultado:* det(D)= 25  

### Ejercicio 2: Regla de Sarrus

$$ E =
\begin{pmatrix}
1 & 2 & 3 \\
0 & 4 & 1 \\
5 & 6 & 0 \\
\end{pmatrix}
$$

#### *Paso 1: Bajar las primeras 2 filas*

$$
\begin{matrix}
1 & 2 & 3 \\
0 & 1 & 4 \\
5 & 6 & 0 \\
1 & 2 & 3 \\
0 & 1 & 4 \\
\end{matrix}
$$

#### *Paso 2: Multiplicar de arriba hacia abajo*
#### (1 x 4 x 0)=0
#### (0 x 6 x 3)=0
#### (5 x 2 x 4)=40

#### *Paso 3: Multiplicar de abajo hacia arriba*
#### -(0 x 2 x 0)=0
#### -(1 x 6 x 4)=-24
#### -(5 x 1 x 3)=-15

#### *Paso 4: Sumar los resultados de la diagonales*
#### 40 - 39= 1
#### *Resultado:* det(E)=1

$$ F =
\begin{pmatrix}
2 & -1 & 3 \\
1 & 4 & 0 \\
3 & 2 & -2 \\
\end{pmatrix}
$$

#### *Paso 1: bajar las primeras 2 filas*

$$
\begin{matrix}
2 & -1 & 3 \\
1 & 4 & 0 \\
3 & 2 & -2 \\
2 & -1 & 3 \\
1 & 4 & 0 \\
\end{matrix}
$$

#### *Paso 2: Multiplicar de arriba hacia abajo*
#### (2 x 4 x -2)=-16
#### (1 x 2 x 3)=6
#### (3 x -1 x 0)=0

#### *Paso 3: Multiplicar de abajo hacia arriba*
#### -(1 x -1 x -2)= -2
#### -(2 x 2 x 0)=0
#### -(3 x 4 x 3)=-36

#### *Paso 4: Sumar los resultados de la diagonales*
#### -52 + 6=1
#### *Resultado:* det(F)= -48

### Ejercicio 3: Método de cofactores

$$ G =
\begin{pmatrix}
1 & 0 & 2 \\
-1 & 3 & 1 \\
2 & 0 & 1 \\
\end{pmatrix}
$$

#### *Paso 1: A la primera columna se le agrega el signo +, y se va alternando el signo*

$$ G =
\begin{pmatrix}
(+) & (-) & (+) \\
1 & 0 & 2 \\
-1 & 3 & 1 \\
2 & 0 & 1 \\
\end{pmatrix}
$$

#### *Paso 2: Aplicar la expansión por cofactores en la primera fila.* 
#### Se multiplica cada elemento de la primera fila por el determinante de su menor correspondiente, respetando el signo (+,-,+) asignado previamente:

$$ det(G) = 1
\begin{bmatrix}
3 & 1 \\
0 & 1 \\
\end{bmatrix}  - 0
\begin{bmatrix}
-1 & 1 \\
2 & 1 \\
\end{bmatrix} +2
\begin{bmatrix}
-1 & 3 \\
2 & 0 \\
\end{bmatrix}
$$

#### Paso 3: Multiplicar y sumar los resultados
#### det(G) = 1 (3 - 0) - 0 (-1 - 2)+ 2(0 - 6)
#### = 3 - 12
#### = -9

#### *Respuesta:* det(G) = -9

### Ejercicio 4: Verificar propiedades 
#### Dadas A y B, Verifica que:

- **det(AB) = det(A) x det(B)**

#### det(AB)=

$$ A =
\begin{pmatrix}
2 & 1 \\
1 & 3 \\
\end{pmatrix}
$$

$$ B =
\begin{pmatrix}
1 & 2 \\
3 & 1 \\
\end{pmatrix}
$$

#### *Paso 1: Multiplicar la matriz A por la Matriz B*

$$ AB =
\begin{bmatrix}
2 * 1 & 2 * 2 \\
1 * 3 & 1 * 1 \\
1 * 1 & 1 * 2 \\
3 * 3 & 3 * 1 \\
\end{bmatrix}
$$

#### *Paso 2: Sumar el resultado de las multiplicaciones.* 
$$ AB =
\begin{bmatrix}
2 + 3 & 4 + 1 \\
1 + 9 & 2 + 3 \\
\end{bmatrix}
$$

#### *Paso 3: Se escribe la matriz*
$$ AB =
\begin{pmatrix}
5 & 5 \\
10 & 5 \\
\end{pmatrix}
$$

#### `Calcular la determinanate de AB`
#### *Paso 4: Multiplicar diagonales*
#### 5 x 5 = 25
#### -(5 x 10)= -50
#### *Paso 5: Sumar los resultados de las multiplicaciones*
#### 25-50=-25
#### *Respuesta:* det(AB)=-25

#### `det(A) x det(B)`

$$ A =
\begin{pmatrix}
2 & 1 \\
1 & 3 \\
\end{pmatrix}
$$

#### `Calcular la determinante de A`
#### *Paso 1: Multiplicar diagonales*
#### 2 x 3 = 6
#### -(1 x 1)= -1
#### *Paso 2: Sumar los resultados de las multiplicaciones*
#### 6-1=5
#### *Resultado:* det(A)=5

$$ B =
\begin{pmatrix}
1 & 2 \\
3 & 1 \\
\end{pmatrix}
$$

#### `Calcular la determinanate de B`
#### *Paso 1: Multiplicar diagonales*
#### 1 x 1=1
#### -(3 x 2)=-6
#### *Paso 2: Sumar los resultados de las multiplicaciones*
#### 1-6=-5
#### *Resultado:* det(B)=-5
#### *Paso 3: Multiplicar las determinanates de A y B*
#### det(A) x det(B) = 5 x -5 = -25

#### `COMPARAR LA DETERMINANTE DE AB Y DE A x B`
#### det(AB) = det(A) x det(B)
#### -25=-25
#### Se comprueba que son iguales

- **det(A ^T)= det(A)**

$$ A =
\begin{pmatrix}
2 & 1 \\
1 & 3 \\
\end{pmatrix}
$$

#### `Calcular la determinanate de A`
#### *Paso 1: Multiplicar diagonales*
#### 2 x 3 = 6
#### -(1 x 1)= -1
#### *Paso 2: Sumar los resultados de las multiplicaciones*
#### 6-1=5
#### *Resultado:* det(A)=5

#### `Escribir la transpuesta de A`

$$ A ^T =
\begin{pmatrix}
2 & 1 \\
1 & 3 \\
\end{pmatrix}
$$
#### `Calcular la determinanate de A ^T
#### *Paso 1: Multiplicar diagonales*
#### 2 x 3 = 6
#### -(1 x 1)= -1
#### *Paso 2: Sumar los resultados de las multiplicaciones*
#### 6-1=5
#### *Resultado:* det(A ^T)=5

#### `Comparamos`
#### det(A ^T)=det(A)
#### 5=5
#### Se comprueba que son iguales

### Ejercicio 5: Aplicaciones geometricas 

#### Dados los vectores u=(3,2) y v=(1,4)
#### a) Calcula el área del paralelogramo que forman 

$$ A =
\begin{pmatrix}
3 & 2 \\
1 & 4 \\
\end{pmatrix}
$$

#### `Calcular la determinanate de A`
#### *Paso 1: Multiplicar diagonales*
#### 3 x 4 = 12
#### -(1 x 2)= -2
#### *Paso 2: Sumar los resultados de las multiplicaciones*
#### 10 - 12 = 10
#### *Resultado:* det(A)=10
#### `El Area es:` Area=10

#### b) ¿Cambia el área si intercambias los vectores?

#### `Paso 1: Intercambiar vectores`
$$ A =
\begin{pmatrix}
3 & 2 \\
1 & 4 \\
\end{pmatrix} => \\ B = 
\begin{pmatrix}
1 & 4 \\
3 & 2 \\
\end{pmatrix} 
$$ 

#### `Calcular la determinanate de B`
#### *Paso 1: Multiplicar diagonales*
#### 1 x 2 = 2
#### -(3 x 4)=-12
#### *Paso 2: Sumar los resultados de las multiplicaciones*
#### -12 + 2=-10
#### *Resultado:* det(B) = -10
#### `El Area es:` Area = -10
#### El area cambia, porque en un inicio el area era igual a 10, y ahora es igual a -10.

#### c) ¿Qué representa el signo del teterminante?
#### Representa si se colocaron bien los vectores a la hora de sacar la determinante.

