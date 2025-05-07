# Método de los coeficientes indeterminados.

Dado el conjunto de funciones $\{1, x, x^2, \dots, x^n\}$ para un $n$ fijo, se tiene que el espacio vectorial generado como combinación lineal de ellas:

$$
V = \{a_0 + a_1x + a_2x^2 + \dots + a_nx^n\,|\, a_0, a_1, \dots, a_n \in \mathbb{R}\}
$$

es un espacio vectorial en el cual la derivación es una operación interna. ¿Que quiere decir esto? Que si yo cojo cualquier función $f\in V$ se va a cumplir que $f'\in V$. Esto no es algo que se vaya a cumplir en cualquier espacio vectorial de funciones, por ejemplo, en el espacio vectorial generador por la función $f(x) = \frac{1}{x}$:
$$
W= \{\frac{a}{x}\,:\, a\in \mathbb{R}\}
$$
se tiene que la función $f(x)=\frac{1}{x}$ pertenece a $W$ mientras que $f'(x)=-\frac{1}{x^2}$ no.

Si en un espacio vectorial $V$ se tiene que la derivada es una operación interna, entonces también lo será la derivada de cualquier orden, así como cualquier combinación lineal de derivadas. Por lo tanto dada una ecuación diferencial de coeficientes constantes, el operador:

$$
\mathcal{L}(y)=a_2 y'' + a_1 y' + a_0 y
$$
es una aplicación lineal en $V$.
