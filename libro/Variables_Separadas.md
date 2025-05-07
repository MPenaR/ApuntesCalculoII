# Ecuaciones en variables separadas

Dada una curva $\Gamma\subset \mathbb{R}^2$ parametrizada por la función:

$$
\mathbf{r}(t) = \left(r_x(t), r_y(t)\right)
$$




$$
\frac{dy}{dx} = \frac{M(y)}{N(x)}
$$

Si $M(y)\neq0$ podemos dividir por $M(y)$ a ambos lados, con lo que obtenemos una ecuación equivalente: 

$$
\frac{1}{M(y)}\frac{dy}{dx} = \frac{1}{N(x)}
$$

Podemos integrar formalmente a ambos lados con respecto a $x$, obteniendo:

$$
\int \frac{1}{M(y(x))}\frac{dy(x)}{dx}\,\mathrm{d}x - \int\frac{1}{N(x)}\,\mathrm{d}x = C
$$

La integral de $N(x)$ no presenta ningún problema, pues la función $N$ es un dato, mientras que el primer término tendríamos que calcular la integral de una función desconocida, pues $y(x)$ es una incógnita. Sin embargo, lo que sí podemos hacer es aplicar el [teorema del cambio de variable](tcv), para reescribirla como:

$$
\int \frac{1}{M(y)}{dy}\,\mathrm{d}x - \int\frac{1}{N(x)}\,\mathrm{d}x = C
$$

En este punto se dice que hemos reducido a cuadraturas la EDO original, pues formalmente ya está resuelta, pues está expresada como integrales simples de funciones conocidas. Lo único que queda es calcular dichas integrales, lo cual se puede hacer de manera exacta o numérica.