# Curvas

En esta asignatura vamos a llamar __curva__ a una parametrización que va de intervalo $I$ (abierto o cerrado) de $\mathbb{R}$ a $\mathbb{R}^2$ o $\mathbb{R}^3$. Este intervalo puede ser no acotado, es decir, puede ser $I=(a,\infty)$ o incluso $I=\mathbb{R}$. En otras ramas de las matemáticas se restringe la definición de curva al caso en el que $I$ Es un intervalo abierto, pero para los conceptos que vamos a estudiar esto no va a ser importante.

## Parametrización

## Reparametrización

## Vector tangente

:::{prf:definition} Vector tangente
Dada una curva $\Gamma$ parametrizada por $\mathbf{r}:I\to\mathbb{R}^d$ llamamos vector tangente en el punto $x_0=\mathbf{x}(t_0)$ al vector:

$$
\mathbf{r}'(t_0)=\left.\frac{d\mathbf{r}}{dt}\right\vert_{t=t_0} = \lim_{h\to 0} \frac{\mathbf{r}(t_0+h) - \mathbf{r}(t_0)}{h}
$$
:::

Si el vector $\mathbf{r}(t)$ está escrito en coordenadas cartesianas:

$$
\mathbf{r}(t) = x(t)\mathbf{i} + y(t)\mathbf{j}
$$

entonces tenemos que :

$$
\mathbf{r}'(t) = \lim_{h\to 0}\frac{x(t+h)\mathbf{i} + y(t+h)\mathbf{j} - x(t)\mathbf{i} + y(t)\mathbf{j}}{h}=\lim_{h\to 0}\frac{x(t+h)-x(t)}{h}\mathbf{i} + \lim_{h\to 0}\frac{y(t+h)-y(t)}{h}\mathbf{j}
$$

lo cual se puede resumir como:

$$
\frac{d}{dt}\left(\begin{array}{c} x(t) \\ y(t) \end{array}\right) = \left(\begin{array}{c} x'(t) \\ y'(t) \end{array}\right)
$$