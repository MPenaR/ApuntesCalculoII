# Integrales de línea

Una integral de línea es una integral de trayectoria en la cual la cantidad a acumular es el producto escalar entre un campo vectorial y el vector tangente unitario a una curva.

(integral_de_linea)=
:::{prf:definition} Integral de línea
Dada una curva $\Gamma\subset\mathbb{R}^d$ y un campo vectorial $\mathbf{F}:\Gamma\to\mathbb{R}^d$, llamamos integral de línea de $\mathbf{F}$ sobre $\Gamma$ a la cantidad:

$$
\int_\Gamma \mathbf{F}\cdot\mathrm{d}\boldsymbol{\ell} := \int_{\Gamma} \mathbf{F}\cdot \mathbf{n}\,\mathrm{d}\ell=\int_a^b \mathbf{F}(\mathbf{r}(t))\cdot \mathbf{r}'(t)\,\mathrm{d}t
$$

:::

:::{prf:property}
La integral de línea de un campo vectorial sobre una curva sí que depende de la parametrización usada para recorrer la curva. En particular, la integral de línea será la misma para reparametrizaciones que no cambian la orientación de la curva y será el mismo valor multiplicado por $-1$ para reparametrizaciones con la orientación contraria.
:::