# Cono de un morfismo
Sea ${}f:A \to B{}$ un [[morfismo de cadenas]]. Llamamos *cono de ${}f{}$*, ${}\text{cone}(f)$ al [[complejo de cadenas]] cuya componente en grado ${}n{}$ es ${}A_{n-1}\oplus B_{n}{}$ y cuyo diferencial viene dado por la siguiente matriz: 
$$
d_{n} = \begin{pmatrix}
-\delta_{n-1} & 0 \\
-f_{n-1} & \partial_{n}
\end{pmatrix}, \text{ donde $\delta$ es el diferencial de $A$ y $\partial$ es el diferencial de $B$}.
$$
En efecto, notemos que:
$$
\begin{align}
d_{n-1}d_{n} &  = \begin{pmatrix}
-\delta_{n-2}  & 0 \\
-f_{n-2} & \partial_{n-1}
\end{pmatrix}\begin{pmatrix}
-\delta_{n-1} & 0 \\
-f_{n-1} & \partial_{n}
\end{pmatrix} = \begin{pmatrix}
\delta_{n-2}\delta_{n-1} & 0 \\
f_{n-2}\delta_{n-1}-\partial_{n-1}f_{n-1} & \partial_{n-1}\partial_{n}
\end{pmatrix} \\
 & =\begin{pmatrix}
 0 & 0 \\
 0 & 0
 \end{pmatrix}
\end{align}
$$

**TODO: Revisar lo anterior usando propiedades universales y diagramas, no elementos.**
## Proposición
Dado un [[morfismo de cadenas]] ${}f:A \to B{}$, existe la siguiente [[sucesión exacta]] corta:
$${}0\to B \overset{\iota}\to \text{cone}(f)\overset\pi\to A[-1]\to 0{}$$
Donde ${}\iota{}$ y ${}\pi{}$ son la inclusión y la proyección obvias.
### Demostración
Como para cada ${}n\in \mathbb{Z}{}$ es trivial, para los morfismos de cadenas completos también.
## Lema
A partir de la [[sucesión exacta]] corta anterior, tenemos la [[sucesión exacta]] larga de [[homología]] (teniendo en cuenta que ${}H_{n+1}(A[-1]) \cong H_{n}(A){}$). El morfismo conector de dicha sucesión es ${}f_{*}{}$.
### Demostración
**TODO**
## Corolario
Un [[morfismo de cadenas]] ${}f{}$ es un [[cuasi-isomorfismo]] si y solo si su cono es exacto.