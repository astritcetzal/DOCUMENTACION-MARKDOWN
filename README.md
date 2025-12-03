# Tecnológico de Software
## Materia: Fundamentos de álgebra
## 3/12/2025
## Alumno: Astrit Airan Cetzal Cetzal
## Actividad \#22 - Matrices

----
### Para esta actividad resolvimos ejercicios que implican matrices, esto con el fin de documentarlo. Apartir de varios metodos (Gauss, Gauss Jordan,inversa, Cramer) encontramos los valores de X, Y y Z . 

### Ejercicio 1: Resolver con todos los metodos 

##### Gaus 

$$
\begin{Bmatrix}
x & + y & + z\\ =6 \\
2x & -y & + z\\ =3 \\
x & 2y & -z\\ =2 \\
\end{Bmatrix}
$$

- Matriz aumentada

$$
\begin{bmatrix}
1 & 1 & 1\\
2 & -1 & 1\\
1 & 2 & -1\\
\end{bmatrix}
\begin{bmatrix}
-1 \\
3 \\
2 \\
\end{bmatrix}
$$

2. Matriz Diagonal: porque todos los elementos fuera de la diagonal principal son cero.

$$ B =
\begin{pmatrix}
3 & 0 & 0 \\
0 & -2 & 0 \\
0 & 0 & 5 \\
\end{pmatrix}
$$

3. Matriz Cuadrada: porque tiene el mismo número de filas y de columnas.

$$ C =
\begin{pmatrix}
2 & 1 & 4 \\
1 & 3 & 5 \\
4 & 5 & 6 \\
\end{pmatrix}
$$

4. Matriz triangular superior: porque todos los elementos de la diagonal principal son cero.

$$ D =
\begin{pmatrix}
1 & 2 & 3 \\
0 & 4 & 5 \\
0 & 0 & 6 \\
\end{pmatrix}
$$

--------------------------------------
### Ejercicio 2: operaciones básicas

##### Para este ejercico se realiza una suma, resta, multiplicaciones y la transpuesta de matrices.

#### a) Suma de A + B

$$ A =
\begin{pmatrix}
2 & -1 \\
3 & 4 \\
\end{pmatrix}
$$

$$ B =
\begin{pmatrix}
5 & 2 \\
-1 & 3 \\
\end{pmatrix}
$$

- Sumar A y B

$$ A + B =
\begin{pmatrix}
2 + 5 & -1 + 2 \\
3 + (-1) & 4 + 3 \\
\end{pmatrix}
$$

- Resultado:

$$ A + B =
\begin{pmatrix}
7 & 1 \\
2 & 7 \\
\end{pmatrix}
$$


#### b) Resta de 2A - B

$$ A =
\begin{pmatrix}
2 & -1 \\
3 & 4 \\
\end{pmatrix}
$$

$$ B =
\begin{pmatrix}
5 & 2 \\
-1 & 3 \\
\end{pmatrix}
$$

1. Multiplicar la matriz A por 2

$$ 2A =
\begin{pmatrix}
2 * 2 & 2 * -1 \\
2 * 3 & 2 * 4 \\
\end{pmatrix}
$$ 

$$ 2A =
\begin{pmatrix}
4 & -2 \\
6 & 8 \\
\end{pmatrix}
$$ 

2. Restar 2A - B

$$ 2A - B =
\begin{pmatrix}
4 - 5 & -2 - 2 \\
6 - (-1) & 8 - 3 \\
\end{pmatrix}
$$

3. Resultado:

$$ 2A - B =
\begin{pmatrix}
-1 & -4 \\
7 & 5 \\
\end{pmatrix}
$$

#### c) AB

$$ A =
\begin{pmatrix}
2 & -1 \\
3 & 4 \\
\end{pmatrix}
$$

$$ B =
\begin{pmatrix}
5 & 2 \\
-1 & 3 \\
\end{pmatrix}
$$

- Multiplicar A por B
  
$$ AB =
\begin{bmatrix}
2 * 5 & 2 * 2 \\
-1 * -1 & -1 * 3 \\
                  \\
3 * 5 & 3 * 2 \\
4 * -1 & 4 * 3 \\
\end{bmatrix}
$$

- Resultado:

$$ AB =
\begin{pmatrix}
11 & 1 \\
11 & 18 \\
\end{pmatrix}
$$

#### d) BA

$$ B =
\begin{pmatrix}
5 & 2 \\
-1 & 3 \\
\end{pmatrix}
$$

$$ A =
\begin{pmatrix}
2 & -1 \\
3 & 4 \\
\end{pmatrix}
$$

- Multiplicar B por A

$$ BA =
\begin{bmatrix}
5 * 2 & 5 * -1 \\
2 * 3 & 2 * 4 \\
                  \\
-1 * 2 & -1 * -1 \\
3 * 3 & 3 * 4 \\
\end{bmatrix}
$$

- Resultado:

$$ BA =
\begin{pmatrix}
16 & 3 \\
7 & 13 \\
\end{pmatrix}
$$

#### e) A^T

$$ A =
\begin{pmatrix}
2 & -1 \\
3 & 4 \\
\end{pmatrix}
$$

- Resultado:

$$ A^T =
\begin{pmatrix}
2 & 3 \\
-1 & 4 \\
\end{pmatrix}
$$

------

### Ejercicio 3: multiplicación en cadena

##### Para este ejercicio se busca desmotrar que la propiedad (AB)C = A(BC) se cumple.

#### Verifique que (AB)C = A(BC)

$$ A =
\begin{pmatrix}
1 & 2 \\
3 & 3 \\
\end{pmatrix}
$$

$$ B =
\begin{pmatrix}
2 & 0 \\
1 & 3 \\
\end{pmatrix}
$$

$$ C =
\begin{pmatrix}
1 & 1 \\
0 & 2 \\
\end{pmatrix}
$$


1. Multiplicar AB

$$ AB =
\begin{bmatrix}
1 * 2  & 1 * 0 \\
2 * 1 & 2 * 3 \\
      \\
3 * 2  & 3 * 0 \\
4 * 1 & 4 * 3 \\
\end{bmatrix}
$$

2. Sumar el resultado de AB

$$ AB =
\begin{bmatrix}
2 + 2  & 6 \\
6 + 4 & 12 \\
\end{bmatrix}
$$

3. Resultado de AB
   
$$ AB =
\begin{pmatrix}
4  & 6 \\
10 & 12 \\
\end{pmatrix}
$$

4. Multiplicar (AB)C

$$ (AB)C =
\begin{bmatrix}
4 * 1  & 4 * 1 \\
6 * 0 & 6 * 2 \\
      \\
10 * 1 & 10 * 1 \\
12 * 0 & 12 * 2 \\
\end{bmatrix}
$$

5. Sumar el resultado de AB por C

$$ (AB)C =
\begin{bmatrix}
4  & 4 + 12 \\
10 & 10 + 24 \\
\end{bmatrix}
$$

6. Resultado de (AB)C
   
$$ (AB)C =
\begin{pmatrix}
4  & 16 \\
10 & 34 \\
\end{pmatrix}
$$

7. Multiplicar BC 

$$ BC =
\begin{bmatrix}
2 * 1  & 2 * 1 \\
0 * 0 & 0 * 2 \\
      \\
1 * 1  & 3 * 0 \\
3 * 0 & 3 * 2 \\
\end{bmatrix}
$$

8. Sumar el resultado de BC
   
$$ BC =
\begin{bmatrix}
2 & 2 \\
1 & 1 + 6 \\
\end{bmatrix}
$$

9. Resultado de BC
   
$$ BC =
\begin{pmatrix}
2  & 2 \\
1 & 7 \\
\end{pmatrix}
$$

10. Multiplicar (BC)A

$$ (BC)A =
\begin{bmatrix}
1 * 2  & 1 * 2 \\
2 * 1 & 2 * 7 \\
      \\
3 * 2 & 3 * 2 \\
4 * 1 & 4 * 7 \\
\end{bmatrix}
$$

11. Sumar el resultado de BC por A

$$ (BC)A =
\begin{bmatrix}
2 + 2 & 2 + 14 \\
6 + 4 & 6 + 28 \\
\end{bmatrix}
$$

12. Resultado de (BC)A
   
$$ (BC)A =
\begin{pmatrix}
4  & 16 \\
10 & 34 \\
\end{pmatrix}
$$

#### 13. Podemos conluir que (AB)C = A(BC)
- Resultado de (AB)C

$$ (AB)C =
\begin{pmatrix}
4  & 16 \\
10 & 34 \\
\end{pmatrix}
$$

- Resultado de (BC)A

$$ (AB)C =
\begin{pmatrix}
4  & 16 \\
10 & 34 \\
\end{pmatrix}
$$
