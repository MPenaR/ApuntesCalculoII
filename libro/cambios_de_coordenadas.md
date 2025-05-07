# Cambios de coordenadas en integrales dobles


## Coordenadas polares

Dado un punto $(x,y)\in\mathbb{R}^2\setminus \{(0,0)\}$, podemos calcular su distancia al origen $r=\sqrt{x^2 +y^2}$ y el ángulo que forma el vector $(x,y)$ con el origen $\theta=\arctan{\frac{y}{x}}$.

DIBUJO

Llamamos coordenadas polares al par $(\rho,\theta)\in\left(0,\infty\right)\left[0,2\pi\right)$ que nos permite identificar a cada punto del plano $\mathbb{R}^2$


## Diferencial de longitud


## Diferencial de área

Teniendo en cuenta que el área de un sector de circunferencia de radio $r$ y ángulo $\alpha$ viene dada por:

$$
A(r,\alpha) = \frac{\alpha r^2}{2}
$$

Podemos calcular el área del diferencial de área $dA$ como la diferecia entre el área de un sector de radio $r+dr$ y ángulo $d\theta$ y el área de un sector de radio $r$ y ángulo $d\theta$

$$
dA = \frac{(r+dr)^2d\theta}{2} - \frac{r^2d\theta}{2} = \frac{r^2d\theta}{2} + rdrd\theta + \frac{dr^2d\theta}{2} - \frac{r^2d\theta}{2} = rdrd\theta + \frac{dr^2d\theta}{2}
$$

Este último resultado, utilizando la [notación de Landau](#landau) se puede reescribir como:

$$
dA = r dr d\theta + o(dr)\quad \text{cuando }dr\to 0
$$

Podemos comprobar que el diferencial de área se podría obtener como el producto de los diferenciales de longitud

$$
dA = d\ell_r d\ell_\theta = dr r d\theta 
$$

Esto se debe a que las coordenadas polares son un tipo de coordenadas curvilíneas en el que todas las curvas coordenadas se cortan formando ángulos rectos. Por ello se dice que son un sistema de coordenadas ortogonal.

## Cambio de coordenadas general