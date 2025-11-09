# Tecnológico de Software
## Materia: Fundamentos de álgebra
## 11/11/2025
## Alumno: Astrit Airan Cetzal Cetzal
## Actividad \#16 - Matrices doc

---
### Ejercicio 1: clasificar matrices

Matriz identidad: porque la diagonal está compuestos por solo unos y los elementos fuera de la diagonal son ceros.

$$ A =
\begin{pmatrix}
1 & 0 \\
0 & 1 \\
\end{pmatrix}
$$

Matriz Diagonal: porque todos los elementos fuera de la diagonal principal son cero.

$$ B =
\begin{pmatrix}
3 & 0 & 0 \\
0 & -2 & 0 \\
0 & 0 & 5 \\
\end{pmatrix}
$$

Matriz Cuadrada: porque tiene el mismo número de filas y de columnas.

$$ C =
\begin{pmatrix}
2 & 1 & 4 \\
1 & 3 & 5 \\
4 & 5 & 6 \\
\end{pmatrix}
$$

Matriz triangular superior: porque todos los elementos de la diagonal principal son cero.

$$ D =
\begin{pmatrix}
1 & 2 & 3 \\
0 & 4 & 5 \\
0 & 0 & 6 \\
\end{pmatrix}
$$

--------------------------------------
### Ejercicio 2: operaciones básicas

#### Suma de A + B

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

$$ A + B =
\begin{pmatrix}
2 + 5 & -1 + 2 \\
3 + (-1) & 4 + 3 \\
\end{pmatrix}
$$

$$ A + B =
\begin{pmatrix}
7 & 1 \\
2 & 7 \\
\end{pmatrix}
$$


#### Resta de 2A - B

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

Multiplicar la matriz A por 2

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

Restar 2A - B

$$ 2A - B =
\begin{pmatrix}
4 - 5 & -2 - 2 \\
6 - (-1) & 8 - 3 \\
\end{pmatrix}
$$

$$ 2A - B =
\begin{pmatrix}
-1 & -4 \\
7 & 5 \\
\end{pmatrix}
$$

#### AB

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

$$ AB =
\begin{pmatrix}
2 * 5 & 2 * 2 \\
-1 * -1 & -1 * 3 \\
                  \\
3 * 5 & 3 * 2 \\
4 * -1 & 4 * 3 \\
\end{pmatrix}
$$

$$ AB =
\begin{pmatrix}
11 & 1 \\
11 & 18 \\
\end{pmatrix}
$$

#### BA

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

$$ BA =
\begin{pmatrix}
5 * 2 & 5 * -1 \\
2 * 3 & 2 * 4 \\
                  \\
-1 * 2 & -1 * -1 \\
3 * 3 & 3 * 4 \\
\end{pmatrix}
$$

$$ BA =
\begin{pmatrix}
16 & 3 \\
7 & 13 \\
\end{pmatrix}
$$




#### A^T

$$ A =
\begin{pmatrix}
2 & -1 \\
3 & 4 \\
\end{pmatrix}
$$

$$ A^T =
\begin{pmatrix}
2 & 3 \\
-1 & 4 \\
\end{pmatrix}
$$

------

### Ejercicio 3: multiplicación en cadena

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

$$ B =
\begin{pmatrix}
1 & 1 \\
0 & 2 \\
\end{pmatrix}
$$


AB

$$ AB =
\begin{pmatrix}
1 * 2  & 1 * 0 \\
2 * 1 & 2 * 3 \\
      \\
3 * 2  & 3 * 0 \\
4 * 1 & 4 * 3 \\
\end{pmatrix}
$$

$$ AB =
\begin{pmatrix}
2 + 2  & 6 \\
6 + 4 & 12 \\
\end{pmatrix}
$$

$$ AB =
\begin{pmatrix}
4  & 6 \\
10 & 12 \\
\end{pmatrix}
$$

(AB)C

$$ (AB)C =
\begin{pmatrix}
4 * 1  & 4 * 1 \\
6 * 0 & 6 * 2 \\
      \\
10 * 1 & 10 * 1 \\
12 * 0 & 12 * 2 \\
\end{pmatrix}
$$

$$ (AB)C =
\begin{pmatrix}
4  & 4 + 12 \\
10 & 10 + 24 \\
\end{pmatrix}
$$

$$ (AB)C =
\begin{pmatrix}
4  & 16 \\
10 & 34 \\
\end{pmatrix}
$$

BC

$$ BC =
\begin{pmatrix}
2 * 1  & 2 * 1 \\
0 * 0 & 0 * 2 \\
      \\
1 * 1  & 3 * 0 \\
3 * 0 & 3 * 2 \\
\end{pmatrix}
$$

$$ BC =
\begin{pmatrix}
2 & 2 \\
1 & 1 + 6 \\
\end{pmatrix}
$$

$$ BC =
\begin{pmatrix}
2  & 2 \\
1 & 7 \\
\end{pmatrix}
$$

(BC)A

$$ (BC)A =
\begin{pmatrix}
1 * 2  & 1 * 2 \\
2 * 1 & 2 * 7 \\
      \\
3 * 2 & 3 * 2 \\
4 * 1 & 4 * 7 \\
\end{pmatrix}
$$

$$ (AB)C =
\begin{pmatrix}
2 + 2 & 2 + 14 \\
6 + 4 & 6 + 28 \\
\end{pmatrix}
$$

$$ (AB)C =
\begin{pmatrix}
4  & 16 \\
10 & 34 \\
\end{pmatrix}
$$

#### Podemos conluir que (AB)C = A(BC)

$$ (AB)C =
\begin{pmatrix}
4  & 16 \\
10 & 34 \\
\end{pmatrix}
$$

$$ (AB)C =
\begin{pmatrix}
4  & 16 \\
10 & 34 \\
\end{pmatrix}
$$







