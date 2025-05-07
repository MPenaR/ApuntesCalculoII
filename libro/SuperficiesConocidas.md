# Parametrizaciones de algunas superficies conocidas

Aquí incluimos algunas parametrizaciones de superficies típicas.

## Cono

Un cono elíptico de eje $Oz$ viene dado por la ecuación implícita:

\begin{equation*}
z^2 = \left(\frac{x}{a}\right)^2 + \left(\frac{y}{b}\right)^2
\end{equation*}

donde $a$ y $b$ son los semiejes de la elipse que se genera al seccionar el cono por el plano $z=1$. Si despejamos $z$ de la ecuación anterior obtenemos automáticamente parametrizaciones del semicono superior $z=\sqrt{\left(\frac{x}{a}\right)^2 + \left(\frac{y}{b}\right)^2}$ y del semicono inferior $z=-\sqrt{\left(\frac{x}{a}\right)^2 + \left(\frac{y}{b}\right)^2}$.

Otra opción es tener en cuenta que se trata de una superficie de revolución de eje de simetría el eje $Oz$

\begin{equation*}
\begin{cases}
x(u,v) = |u| \cos(v)\\
y(u,v) = |u| \sin(v)\\
z(u,v) = u
\end{cases}
\end{equation*}

## Hiperboloide de una hoja

\begin{equation*}
x^2 + y^2 = z^2 + K^2
\end{equation*}

\begin{equation*}
\begin{cases}
x(u,v) = \sqrt{u^2 + K^2}\cos(v)\\
y(u,v) = \sqrt{u^2 + K^2}\sin(v)\\
z(u,v) = u
\end{cases}
\end{equation*}

\begin{equation*}
\begin{cases}
x(u,v) = K\cosh(u)\cos(v)\\
y(u,v) = K\cosh(u)\sin(v)\\
z(u,v) = K\sinh(u)
\end{cases}
\end{equation*}

## Hiperboloide de dos hojas

\begin{equation*}
x^2 + y^2 = z^2 - K^2
\end{equation*}

\begin{equation*}
\begin{cases}
x(u,v) = \sqrt{u^2 - K^2}\cos(v)\\
y(u,v) = \sqrt{u^2 - K^2}\sin(v)\\
z(u,v) = u
\end{cases}
\end{equation*}

$u>K$ o $u< -K$.


\begin{equation*}
\begin{cases}
x(u,v) = K\sinh(u)\cos(v)\\
y(u,v) = K\sinh(u)\sin(v)\\
z(u,v) = K\cosh(u)
\end{cases}
\end{equation*}

$u>0$ o


\begin{equation*}
\begin{cases}
x(u,v) = K\sinh(u)\cos(v)\\
y(u,v) = K\sinh(u)\sin(v)\\
z(u,v) = -K\cosh(u)
\end{cases}
\end{equation*}
