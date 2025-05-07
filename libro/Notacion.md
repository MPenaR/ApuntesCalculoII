# Notación

## Igualdades, definiciones e identidades.

En matemáticas se pueden encontrar tres signos de igual, muy parecidos que pueden generar confusión. El signo $=$ se usa para imponer igualdad entre dos cantidades. Por ejemplo podemos buscar la solución real a la ecuación

$$
x^2 - 2x + 1 = 0
$$

que se da para $x=1$. Cuando la igualdad se da por definición lo marcaremos con $:=$


## Vectores y matrices.

A lo largo del los apuntes los vectores se denotarán con letras minúsculas en negrita $\mathbf{u},\mathbf{v},\dots$. Se utilizarán las letras $\mathbf{i}$, $\mathbf{j}$ y $\mathbf{k}$ para los 3 vectores unitarios segun los ejes de coordenadas cartesianas, es decir: 

:::{aside}
En la pizarra es difícil marcar de manera consistente la diferencia entre caracteres en negrita y caracteres normales, por lo que en el texto manuscrito normalmente se usará $\vec{u},\vec{v},\dots$ para denotar a los vectores.
:::


$$
\mathbf{i}=(1,0),\,\mathbf{j}=(0,1)
$$
si estamos en $\mathbf{R}^2$ y 
$$
\mathbf{i}=(1,0,0),\,\mathbf{j}=(0,1,0),\,\mathbf{k}=(0,0,1)
$$
si nos encontramos en $\mathbb{R}^3$.


Las matrices se denotarán por letras mayúsculas en negrita.

## Producto cartesiano

(producto_cartesiano)=
:::{prf:definition} Producto cartesiano
Dados dos conjuntos $A$ y $B$ llamamos producto cartesiano $A$ y $B$ y lo denotamos por $A\times B$ al conjunto:

$$
A \times B = \left\{ (a,b)\,:\, a\in A,\, b\in B \right\}
$$
:::

Así, por ejemplo, el plano se identificacon el conjunto de pares $(x,y)$ donde $x$ puede tomar cualquier valor real, e $y$ también, por lo que denotaremos al plano como $\mathbb{R}^2=\mathbb{R}\times\mathbb{R}$.


(landau)=
## Notación de Landau

Si $f$ y $g$ son dos funciones tales que $f(x)\to 0$ y $g(x)\to 0$ cuando $x\to a$ entonces se dice que $f(x)$ es un infinitésimo de orden superior que $g(x)$ y se denota $f(x) = o(g(x))$ si se cumple que:

$$
\lim_{x\to a } \frac{f(x)}{g(x)}
$$

Así, por ejemplo, podemos decir que $x^2 = o(x)$ para $x\to 0$. O que $cos(x - \frac{\pi}{2}) - 1 = o\left(x - \frac{\pi}{2}\right)$ cuando $x\to\frac{\pi}{2}$. Esto último también nos permite decir que:

$$
\cos(x-\frac{\pi}{2}) = 1 + o\left(x - \frac{\pi}{2}\right)\quad\text{cuando }x\to\frac{\pi}{2}
$$


