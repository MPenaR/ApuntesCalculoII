# Gradiente de la función potencial
Sea $\mathbf{x}_O\in\mathbb{R}^2$ un punto fijo y $\mathbf{F}:\mathbb{R}^2 \to \mathbb{R}^2$ un campo vectorial [conservativo](#conservativo). Para cada punto $\mathbf{x}$ podemos definir la función:

$$
f(\mathbf{x}) = \int_{\Gamma_{\mathbf{x}_O\to\mathbf{x}}} \mathbf{F}\cdot\mathrm{d}\boldsymbol{\ell}
$$

donde $\Gamma_{\mathbf{x}_O\to\mathbf{x}}$ denota cualquier curva con inicio $\mathbf{x}_O$ y final en $\mathbf{x}$. 

Dicha función está bien definida, pues al ser $\mathbf{F}$ un campo conservativo, no es necesario especificar qué curva utilizamos para calcular su valor en $\mathbf{x}$, pues cualquier curva que vaya de $\mathbf{x}_O$ a $\mathbf{x}$ nos dará la misma integral.

Vamos a ver qué relación existe entre el gradiente del campo escalar $f$ y el campo vectorial $\mathbf{F}$. Por comodidad vamos a denotar por $U$ y $V$ a las componentes de $\mathbf{F}$, es decir, $\mathbf{F}(\mathbf{x}) = \left(U(x,y), V(x,y)\right)$

La derivada parcial con respecto a $x$ es, por definición:

$$
\lim_{h\to 0} \frac{\rho(x+h,y) - \rho(x,y)}{h}
$$

Del apartado BLA, sabemos que $\rho(x_+h,y) - \rho(x,y)$ coincide con la integral de línea del campo vectorial $\mathbf{F}$ sobre el segmento $[(x,y),(x+h,y)]$  el cual admite la parametrización:

$$
(x(t),y(t)) = (x+th,y),\quad t\in[0,1]
$$

y vector tangente $\mathbf{x}'(t)=\left(h,0\right)$, por lo que se tiene que:


$$
\lim_{h\to 0} \frac{\rho(x+h,y) - \rho(x,y)}{h} =  \lim_{h\to 0} \frac{\int_0^1 \mathbf{F}(\mathbf{x}(t))\cdot (h,0)\mathrm{d}t}{h}=  \lim_{h\to 0} \int_0^1 U(x+th,y)\mathrm{d}t
$$


Ahora, expandiendo $U$ en serie de Taylor cerca de $(x,y)$ se tiene que:

$$
U(x+th,y)=U(x,y) + \frac{\partial U }{\partial x}(x,y)ht + o(h)
$$

con lo que:

$$
\lim_{h\to 0} \frac{\rho(x+h,y) - \rho(x,y)}{h} = \lim_{h\to 0} \int_0^1 \left( U(x,y) + th\frac{\partial U}{\partial x}(x,y)\right)\mathrm{d}t + o(h) = U(x,y)
$$

