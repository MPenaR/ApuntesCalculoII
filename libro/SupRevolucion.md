# Superficies de revolución
(sup_revolucion)=
:::{prf:definition} Superficie de revolución
Decimos que una superficie $S$ es de revolución cuando se puede generar rotando una [curva plana](#curva_plana) al rededor de un eje contenido en dicho plano.
:::

Supongamos que la curva se encuentra en el plano $Oxz$ y el eje de rotación es el eje $Oz$. Si describiésemos la superficie en coordenadas cilíndricas, tendríamos que:

\begin{equation*}
\begin{cases}
r(u,v) = f(u)\\
\theta(u,v) = v\\
z(u,v) = u
\end{cases}
\end{equation*}

Lo cual, al pasarlo a coordenadas cartesianas queda:

\begin{equation*}
\begin{cases}
x(u,v) = f(u)\cos(v)\\
y(u,v) = f(u)\sin(v)\\
z(u,v) = u
\end{cases}
\end{equation*}

y nos da una ecuación del tipo:

\begin{equation*}
z = g(x^2+y^2)
\end{equation*}

<iframe src="paraboloide_eliptico.html">
</iframe>