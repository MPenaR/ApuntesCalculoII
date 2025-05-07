# Independencia lineal y Wronskiano

Dadas dos funciones derivables $f$ y $g$ definimos su Wronskiano como la función:

$$
W(x)=\left|\begin{array}{cc}
f(x) & g(x) \\
f'(x) & g'(x) 
\end{array}\right| = f(x)g'(x) - f'(x)g(x)
$$

Es sencillo demostrar que si existe $k\in\mathbb{R}$ tal que $f(x)=kg(x)$ para todo $x\in\mathbb{R}$, entonces se tiene que $W(x)=0$ para todo $x\in\mathbb{R}$. Es decir, el Wronskiano de dos funciones linealmente dependientes es identicamente nulo. 


:::{prf:theorem}
Sean $y_1$ e $y_2$ dos soluciones de la EDO:

$$
y''(x) + p(x)y'(x) + q(x)y(x) = 0
$$
con $p$ y $q$ funciones continuas.

Si existe un $\xi\in\mathbb{R}$ para el que $W(\xi)=0$, entonces $W(x)=0$ para todo $x\in\mathbb{R}$. 
:::

:::{prf:proof}
Si calculamos la derivada del Wronskiano de $y_1$ e $y_2$ tenemos que:

$$
\frac{dW}{dx} = y_1(x) y''_2(x) - y''_1(x) y_2(x)
$$

Sustituyendo ahora los valores de $y''_1$ e $y''_2$ (por ser soluciones de la ecuación) obtenemos:

$$
\frac{dW}{dx} = y_1(x)\left(-p(x)y'_2(x)-q(x)y_2(x)\right) - \left(-p(x)y'_1(x)-q(x)y_1(x)\right) y_2(x)
$$

es decir

$$
\frac{dW}{dx} = -p(x)\left(y_1(x)y'_2(x) - y'_1(x) y_2(x)\right)=-p(x)W(x)
$$

Esto junto con el hecho de que $W(\xi)=0$ nos permite plantear un problema de valor inicial para el Wronskiano:

$$
\begin{cases}
\frac{dW}{dx}=-p(x)W(x) & x\in \mathbb{R}\\
W(\xi)=0
\end{cases}
$$

Es sencillo comprobar que dicho problema tiene solución única $W(x)=0$.
:::
