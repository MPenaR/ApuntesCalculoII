# Teorema de Green


En esta sección vamos a enunciar y justificar el Teorema de Green, así como dar una condición suficiente para que un campo vectorial sea conservativo.

:::{prf:theorem} Green
Dado un campo vectorial $\mathbf{F}:D\to\mathbb{R}^2$ definido en un conjunto $D\subset{\mathbb{R}^2}$ [simplemente conexo](#simplemente_conexo), se tiene que para cualquier [curva de Jordan](#curva_jordan) $\Gamma\subset D$:

\begin{equation*}
\oint_\Gamma \mathbf{F}\cdot\mathrm{d}\boldsymbol{\ell} = \iint_\Omega \left( \frac{\partial F_y}{\partial x} - \frac{\partial F_x}{\partial y} \right)\,\mathrm{d}S
\end{equation*}

donde $\Omega$ es la región encerrada por la curva $\Gamma$.
:::

En particular, si $\frac{\partial F_y}{\partial x} = \frac{\partial F_x}{\partial y}$ en todo punto de un conjunto simplemente conexo $D$, se tiene que la integral de línea de $\mathbf{F}$ sobre cualquier curva cerrada en $D$ es cero, y por lo tanto $\mathbf{F}$ es un campo conservativo en $D$. 


## Separación de una curva cerrada en varias. 

Sea $\Gamma$ una curva cerrada con la de la figura:


Podemos cortar la curva por otra curva de manera que  (FIGURA) la integral en la curva original es igual a la suma de ambas curvas cerradas, pues:

$$
\oint_{\Gamma_A} \mathbf{F}\cdot\mathrm{d}\boldsymbol{\ell} + \oint_{\Gamma_B} \mathbf{F}\cdot\mathrm{d}\boldsymbol{\ell}  = \int_{\Gamma_1} \mathbf{F}\cdot\mathrm{d}\boldsymbol{\ell} + \int_{\Gamma_3} \mathbf{F}\cdot\mathrm{d}\boldsymbol{\ell} - \int_{\Gamma_3} \mathbf{F}\cdot\mathrm{d}\boldsymbol{\ell} + \int_{\Gamma_2} \mathbf{F}\cdot\mathrm{d}\boldsymbol{\ell}
$$

$$
 =\int_{\Gamma_1} \mathbf{F}\cdot\mathrm{d}\boldsymbol{\ell} + \int_{\Gamma_2} \mathbf{F}\cdot\mathrm{d}\boldsymbol{\ell} = \oint_{\Gamma} \mathbf{F}\cdot\mathrm{d}\boldsymbol{\ell}
$$



### Circulación en un rectángulo "infinitesimal".

Sea el rectángulo de la figura, de lados $l$ y $h$ y centro $(x_0,y_0)$, es decir

$$
\left\{(x,y)\in\mathbb{R}^2\,:\,-\frac{l}{2}\le x \le \frac{l}{2},\,-\frac{h}{2}\le y \le \frac{h}{2}\right\}
$$

Vamos a calcular la circulación del campo $\mathbf{F}(\mathbf{x}) = U(\mathbf{x})\mathbf{i} + V(\mathbf{x})\mathbf{j}$. Para ello separamos la frontera en $4$ curvas formadas por los segmentos rectos: 

- $\Gamma_1$

$$
\mathbf{x}_1(t) = \left(x_0 + tl,\, y_0 - \frac{h}{2}\right),\quad t\in\left[-\frac{1}{2},\frac{1}{2}\right]
$$

$\mathbf{x}'_1(t)=\left(l,0\right)$

$$
\int_{\Gamma_1} \mathbf{F}\cdot\mathrm{d}\boldsymbol{\ell}=l\int_{-\frac{1}{2}}^\frac{1}{2} F_x\left( x_0 + tl,\, y_0 - \frac{h}{2}\right)\,\mathrm{d}t
$$

Ahora, expandiendo $F_x$ en serie de Taylor alrededor del punto $(x_0, y_0)$:

\begin{equation*}
F_x\left(x_0+tl,y_0-\frac{h}{2}\right) = F_x(x_0,y_0) + tl\frac{\partial F_x}{\partial x}(x_0,y_0) - \frac{h}{2}\frac{\partial F_x}{\partial_y}(x_0,y_0) + o\left(\sqrt{h^2 + l^2}\right) 
\end{equation*}

Con lo que

$$
\int_{\Gamma_3} \mathbf{F}\cdot\mathrm{d}\boldsymbol{\ell}=lF_x(x_0,y_0) - l\frac{h}{2} \frac{\partial F_x}{\partial y}(x_0,y_0) + o\left(h^2 + l^2\right) 
$$


- $\Gamma_2$

\begin{equation*}
\mathbf{x}_2(t) = (x_0 + \frac{l}{2},\, y_0 + th),\quad t\in\left[-\frac{1}{2},\frac{1}{2}\right]
\end{equation*}

$$
\mathbf{x}'_2(t) = \left(0,h\right)
$$

\begin{equation*}
F_y\left(x_0+\frac{l}{2},\, y_0 + tl\right)= F_x(x_0,y_0) + \frac{l}{2}\frac{\partial F_y}{\partial x}(x_0,y_0) + th\frac{\partial F_y}{\partial y}(x_0,y_0) + o(\sqrt{l^2 + y^2})
\end{equation*}

$$
\int_{\Gamma_2} \mathbf{F}\cdot\mathrm{d}\boldsymbol{\ell}=hF_y(x_0,y_0) +h\frac{l}{2} \frac{\partial F_y}{\partial x}(x_0,y_0) + o\left(h^2 + l^2\right)
$$


- $\Gamma_3$

\begin{equation*}
\mathbf{x}_3(t) = (x_0 - lt,\, y_0 + \frac{h}{2}),\quad t\in\left[-\frac{1}{2},\frac{1}{2}\right]
\end{equation*}

$$
\mathbf{x}'_3(t) = \left(-l,0\right)
$$

$$
F_x\left(x_0-lt,\, y_0 + \frac{h}{2}\right)= F_x(x_0,y_0) + -tl\frac{\partial F_x}{\partial x}(x_0,y_0) + \frac{h}{2}\frac{\partial F_x}{\partial y}(x_0,y_0) + o\left(\sqrt{l^2 + h^2}\right)
$$

$$
\int_{\Gamma_3} \mathbf{F}\cdot\mathrm{d}\boldsymbol{\ell}=-lF_x(x_0,y_0) - l\frac{h}{2} \frac{\partial F_x}{\partial y}(x_0,y_0) + o\left(h^2 + l^2\right) 
$$

- $\Gamma_4$

\begin{equation*}
\mathbf{x}_4(t) = (x_0 - \frac{l}{2},\, y_0 - ht),\quad t\in\left[-\frac{1}{2},\frac{1}{2}\right]
\end{equation*}

$$
\mathbf{x}'_4(t) = \left(0,-h\right)
$$

$$
F_y\left(x_0-\frac{l}{2},\, y_0 - ht\right)= F_y(x_0,y_0) - \frac{l}{2}\frac{\partial F_y}{\partial x} - ht\frac{\partial F_y}{\partial y}(x_0,y_0) + o\left(\sqrt{l^2 + h^2}\right)
$$

$$
\int_{\Gamma_4} \mathbf{F}\cdot\mathrm{d}\boldsymbol{\ell}=-hF_y(x_0,y_0) + h\frac{l}{2} \frac{\partial F_y}{\partial x}(x_0,y_0) + o\left(\sqrt{h^2 + l^2}\right) 
$$

Con lo que finalmente se tiene que:

$$
\oint_\Gamma \mathbf{F}\cdot\mathrm{d}\boldsymbol{\ell} = lh\left(\frac{\partial F_y}{\partial x} - \frac{\partial F_x}{\partial y}\right) + o\left(h^2 + l^2\right) 
$$

Si ahora sumamos en todos los cuadrados tenemos que 

\begin{equation*}
\oint_{\Gamma} \mathbf{F}\cdot\,\mathrm{d}\boldsymbol{\ell} = \lim_{dx\to 0,\,dy\to 0}\sum \left(\frac{\partial F_y}{\partial x}(x,y) - \frac{\partial F_x}{\partial y}(x,y)\right)dxdy = \iint_{D} \left(\frac{\partial F_y}{\partial x} - \frac{\partial F_x}{\partial y}\right) \,\mathrm{d}A
\end{equation*}
