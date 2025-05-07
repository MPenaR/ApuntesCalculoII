# Integrales de trayectoria

:::{prf:definition} Integral de trayectoria
Dada una curva $\Gamma$ definida por una parametrización $\mathbf{r}:[a,b]\to\mathbb{R}^d$ y un campo escalar $f:\Gamma\to\mathbb{R}$ llamamos integral de trayectoria de $f$ sobre la curva $\Gamma$ a la cantidad:

$$
\int_{\Gamma} f d\ell = \int_a^b f(\mathbf{r}(t))\|\mathbf{r}'(t)\|\,\mathrm{d}t
$$
:::

:::{prf:property}
Las integrales de trayectoria son independientes de la parametrización usada para representar la curva $\Gamma$.
:::

:::{prf:proof}
:class: dropdown
Sean $\mathbf{r}:[a,b]\to\mathbb{R}^d$ y $\mathbf{q}:[c,d]\to\mathbb{R}^d$ dos parametrizaciones de la misma curva $\Gamma$.

Por una parte tenemos que:

$$
\int_{\Gamma} f d\ell = \int_a^b f(\mathbf{r}(t))\|\mathbf{r}'(t)\|\,\mathrm{d}t
$$

Ahora bien, por ser $\mathbf{r}$ y $\mathbf{q}$ dos parametrizaciones de $\Gamma$, entonces existirá una biyección continua $j:[c,d]\to[a,b]$ y de clase $C^\infty$ tal que $\mathbf{q} = \mathbf{r}\circ j$. Haciendo el cambio de variable $t=j(\tau)$ se tiene que

$$
\int_a^b f(\mathbf{r}(t))\|\mathbf{r}'(t)\|\,\mathrm{d}t= \int_{j^{-1}(a)}^{j^{-1}(b)} f(\mathbf{r}(j(\tau)))\|\mathbf{r}'(j(\tau))\|j'(\tau)\,\mathrm{d}\tau
$$

Sin embargo, recordando que $\mathbf{q}=\mathbf{r}\circ j$ tenemos por una parte que:

$$
f(\mathbf{r}(j(\tau))) = f(\mathbf{q}(\tau))
$$

Por otra parte, si $j$ es una reparametrización sin cambio de orientación, entonces $j'(\tau)>0$, $j(c)=a$ y $j(d)=b$ y por lo tanto 

$$
\|\mathbf{q}'(\tau)\| = \|\mathbf{r}'(j(\tau))j'(\tau)\| = \|\mathbf{r}'(j(\tau))\|j'(\tau)
$$

Con lo cual, sustituyendolo en la integral tenemos que:

$$
\int_{j^{-1}(a)}^{j^{-1}(b)} f(\mathbf{r}(j(\tau)))\|\mathbf{r}'(j(\tau))\|\,j'(\tau)\mathrm{d}\tau = \int_c^d f(\mathbf{q}(\tau))\|\mathbf{q}'(\tau)\|\,\mathrm{d}\tau = \int_\Gamma f\,\mathrm{d}\ell
$$

Finalmente, si se tratase de una reparametrización con cambio de orientación, entonces $j'(\tau)<0$, $j(c)=b$ y $j(d)=a$, con lo que

$$
\|\mathbf{q}'(\tau)\| = \|\mathbf{r}'(j(\tau))j'(\tau)\| = -\|\mathbf{r}'(j(\tau))\|j'(\tau)
$$

y

$$
\int_{j^{-1}(a)}^{j^{-1}(b)} f(\mathbf{r}(j(\tau)))\|\mathbf{r}'(j(\tau))\|\,j'(\tau)\mathrm{d}\tau = -\int_d^c f(\mathbf{q}(\tau))\|\mathbf{q}'(\tau)\|\,\mathrm{d}\tau =
$$

Y recordando que en una integral simple intercambiar los límites equivale a multiplicar la integral por $-1$, se tiene que


$$
-\int_d^c f(\mathbf{q}(\tau))\|\mathbf{q}'(\tau)\|\,\mathrm{d}\tau = \int_c^d f(\mathbf{q}(\tau))\|\mathbf{q}'(\tau)\|\,\mathrm{d}\tau = \int_\Gamma f \,\mathrm{d}\ell
$$

Con lo que quedaría demostrado que la integral de trayectoria es independiente de la parametrización.


:::