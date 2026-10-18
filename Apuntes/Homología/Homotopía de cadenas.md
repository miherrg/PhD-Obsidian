# Homotopía nula
Diremos que un [[Morfismo de cadenas]], ${}f : C \to D{}$, es *homotópicamente nulo* si existen morfismos ${}s_{n}:C_{n} \to D_{n+1}{}$ tales que ${}f_{n} = \delta_{n+1}s_{n} + s_{n-1}d_{n}{}$, donde ${}d{}$ y ${} \delta{}$ son los morfismos diferenciales de ${}C{}$ y ${}D{}$, respectivamente.
A los morfismos ${}\{ s_{n} \}_{n\in \mathbb{Z}}{}$ los llamaremos contracciones de cadenas de f.
# Homotopía de cadenas
Diremos que dos [[Morfismo de cadenas|morfismos de cadenas]], ${}f, g : C \to D{}$ son *homótopos* si su diferencia es homotópicamente nula. En este caso, a las contracciones de cadenas de ${}f-g{}$ las llamaremos una *homotopía de cadenas*.
# Equivalencia homotópica de cadenas
Diremos que ${}f:C \to D{}$ es una *equivalencia homotópica de cadenas* si ${}\exists g:D \to C{}$ tal que ${}fg{}$ y ${}gf{}$ son homótopos las identidades correspondientes.

## Lema
Si ${}f:C\to D{}$ es homotópicamente nulo, entonces todo morfismo ${}f_{*}:H_{n}(C)\to H_{n}(D){}$ es nulo.
### Demostración
**TODO**
### Corolario
Si ${}f,g:C\to D{}$ son homótopos entonces inducen el mismo morfismo ${}f_{*} = g_{*}{}$
## Lema
Si ${}F{}$ es un [[Functor aditivo]] y ${}f{}$ es homotópicamente nulo, entonces ${}Ff{}$ también lo es.
### Demostración
**TODO**
### Corolario
Si ${}F{}$ es un [[Functor aditivo]] y ${}f,g{}$ son homótopos, entonces ${}Ff, Fg{}$ también lo son.