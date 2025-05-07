# Campos conservativos y función potencial.

(conservativo)=
:::{prf:definition} Campo conservativo
Dado un campo vectorial $\mathbf{F}:\mathbb{R}^2\to\mathbb{R}^2$  decimos que dicho campo es conservativo en $D\subset\mathbb{R}^2$ si para cualquier curva cerrada $\Gamma \subset D$ se cumple que:

$$
\oint_{\Gamma} \mathbf{F}\cdot\,\mathrm{d}\boldsymbol{\ell} = 0
$$

:::


La definición anterior es equivalente a decir que, dados dos puntos cualesquiera $\mathbf{x}_A$ y $\mathbf{x}_B$, la integral de línea del campo $\mathbf{F}$ sobre cualquier curva que une $\mathbf{x}_A$ con $\mathbf{x}_B$ es la misma. Es decir, su valor no depende de la curva en sí, si no de los puntos inicial y final.

Para demostrarlo, tomamos dos curvas cualesquiera $\Gamma_1$ y $\Gamma_2$ cuyo punto inicial es $\mathbf{x}_A$ y su punto final es $\mathbf{x}_B$. Si consideramos la curva $\Gamma = \Gamma_1 + \Gamma^-_2$  es decir, la curva resultante de concatenar $\Gamma_1$ con $\Gamma_2$ recorrida en sentido inverso tenemos que $\Gamma$ es una curva cerrada, por lo que:

$$
0 = \int_\Gamma \mathbf{F}\cdot\mathrm{d}\boldsymbol{\ell} = \int_{\Gamma_1} \mathbf{F}\cdot\mathrm{d}\boldsymbol{\ell} + \int_{\Gamma^-_2} \mathbf{F}\cdot\mathrm{d}\boldsymbol{\ell}= \int_{\Gamma_1} \mathbf{F}\cdot\mathrm{d}\boldsymbol{\ell} - \int_{\Gamma_2} \mathbf{F}\cdot\mathrm{d}\boldsymbol{\ell}
$$

donde se usó el hecho de que la integral de línea cambia de signo al cambiar la orientación de la curva. 

(function_potencial)=
:::{prf:definition} Función potencial
Decimos que un campo vectorial $\mathbf{F}$ deriva de un potencial si existe un campo escalar $f$ tal que $\mathbf{F}=\nabla{f}$. Se dice que $f$ es una función potencial del campo $\mathbf{F}$.
:::

