# Integrales dobles

## Integrales iteradas

Dada una función escalar de dos variables $f:\mathbb{R}^2 \to \mathbb{R}$, 

$$
\left(x,y\right) \mapsto z = f(x,y)
$$

si fijamos un valor para $y$, por ejemplo $y=a$, obtendremos una nueva función de una sola variable $f_{a}:\mathbb{R}\to\mathbb{R}$

$$
x\mapsto z = f(x,a)
$$

Por ejemplo, en la figura siguiente mostramos las gráficas de las diferentes funciones $f_y$ que se obtienen cuando en la función $f(x,y)=x^2 + y^2$ se fija el valor de $y$.


### Integral doble sobre un rectángulo

Dado un rectángulo $\mathcal{R} = [a,b]\times[c,d]$ y una función $f:\mathbb{R}^2\to\mathbb{R}$, llamaremos integral doble de la función $f$ sobre $\mathcal{R}$ a la cantidad:

DIBUJO

### Interpretación geométrica

La integral doble de una función positiva $f$ sobre una región $\mathcal{R}$ coincide con el volumen del sólido delimitado por la superficie $z=f(x,y)$ y el plano $z=0$ sobre la región $\mathcal{R}$


DIBUJO


Si la función fuese negativa, entonces el valor absoluto de la integral coincidiría con el volumen.

DIBUJO

### Teorema de Fubini

A la hora de calcular la integral doble de una función continua en un rectángulo se puede intercambiar el orden de integración.

:::{prf:theorem} Fubini
Sea $f:\mathbb{R}^2 \to \mathbb{R}$, una función integrable en el rectángulo $\mathcal{R} = [a,b]\times[c,d]$, entonces se tiene que:

$$
\iint_{R} f\,\mathrm{d}S = \int_a^b\left(\int_c^df(x,y)\,\mathrm{d}y\right)\mathrm{d}x = \int_c^d\left(\int_a^bf(x,y)\,\mathrm{d}x\right)\mathrm{d}y
$$
:::

### Integral doble sobre un dominio general

#### Dominios proyectables

:::{prf:definition} Región de tipo I
Diremos que una región es $\mathcal{R}$ de tipo I o proyectable sobre el eje $Ox$  si es posible expresarla como:

$$
\mathcal{R} = \left\{(x,y)\in\mathbb{R}^2\,:\,a \le x \le b,\, g(x) \le y \le h(x) \right\}
$$
:::

DIBUJO de dominio I y dominio que no es de tipo I

:::{prf:definition} Región de tipo II
Diremos que una región es $\mathcal{R}$ de tipo II o proyectable sobre el eje $Oy$  si es posible expresarla como:

$$
\mathcal{R} = \left\{(x,y)\in\mathbb{R}^2\,:\,a \le y \le b,\, g(y) \le x \le h(y) \right\}
$$
:::



### Calculo de integrales dobles

El cálculo de integrales dobles consistirá en transformarlas en integrales iteradas.
