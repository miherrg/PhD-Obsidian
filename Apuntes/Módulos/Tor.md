# Tor
Denotamos por ${}\text{Tor}_{n}^{R}(\_{},N) := L_{n}(\_\otimes_{R} N){} {}$ y por ${}\text{Tor}_{n}^{R}(M,\_) := L_{n}(M\otimes_{R}\_{}){}$. Ambos [[Functor derivado|functores derivados]] existen pues ${}M\otimes_{R}\_{}{}$ y ${}\_{\otimes}_{R}N{}$ son functores exactos a derecha y ${}R{}$-Mod tiene suficientes [[proyectivos#Proposición|proyectivos]].
## Teorema
Sean ${}M,N{}$ ${}R{}$-módulos. ${}\forall n,\; \text{Tor}_{n}^{R}(\_{},N)(M) \cong \text{Tor}_{n}^{R}(M,\_{})(N){}$. Por tanto, podemos hablar del ${}\text{Tor}_{n}^{R}(M,N){}$ y es único salvo isomorfismo.
### Demostración
Sean ${} {}\mathcal{F}\overset{\pi}\to M, \mathcal{G}\overset{\varepsilon}{\to}N{} {}$ resoluciones proyectivas de ${}M, N{}$ con diferenciales ${}\phi, \psi{}$, respectivamente.
Denotamos por ${}\mathcal{F}\otimes \mathcal{G}{}$ el módulo proyectivo ${}\oplus_{i,j}F_{i}\otimes G_{j}{}$. Para cada fila ${}i{}$, definimos el diferencial horizontal ${}(-1)^i\otimes \psi{}$ y para cada columna ${}j{}$, el diferencial vertical ${}\phi\otimes 1{}$. Notemos que como ${}M \otimes\_{}{}$ como ${}\_{}\otimes N{}$ son exactos a derecha, cada fila y cada columna del siguiente diagrama son resoluciones de ${}F_{i}\otimes N{}$ y ${}M \otimes G_{j}{}$.
```cd
{
  "version": 1,
  "rows": 6,
  "cols": 6,
  "cells": [
    {
      "row": 0,
      "col": 1,
      "label": "\\vdots"
    },
    {
      "row": 0,
      "col": 2,
      "label": "\\vdots"
    },
    {
      "row": 0,
      "col": 3,
      "label": "\\vdots"
    },
    {
      "row": 0,
      "col": 5,
      "label": "\\vdots"
    },
    {
      "row": 1,
      "col": 0,
      "label": "\\cdots"
    },
    {
      "row": 1,
      "col": 1,
      "label": "{F_{i+1} \\otimes G_{j+1}}"
    },
    {
      "row": 1,
      "col": 2,
      "label": "F_{i+1} \\otimes G_{j}"
    },
    {
      "row": 1,
      "col": 3,
      "label": "{F_{i+1} \\otimes G_{j-1}}"
    },
    {
      "row": 1,
      "col": 4,
      "label": "\\cdots"
    },
    {
      "row": 1,
      "col": 5,
      "label": "{F_{i+1}\\otimes N}"
    },
    {
      "row": 2,
      "col": 0,
      "label": "\\cdots"
    },
    {
      "row": 2,
      "col": 1,
      "label": "F_i \\otimes G_{j+1}"
    },
    {
      "row": 2,
      "col": 2,
      "label": "{F_i \\otimes G_{j}}"
    },
    {
      "row": 2,
      "col": 3,
      "label": "F_i \\otimes G_{j-1}"
    },
    {
      "row": 2,
      "col": 4,
      "label": "\\cdots"
    },
    {
      "row": 2,
      "col": 5,
      "label": "{F_{i+1}\\otimes N}"
    },
    {
      "row": 3,
      "col": 0,
      "label": "\\cdots"
    },
    {
      "row": 3,
      "col": 1,
      "label": "{F_{i-1} \\otimes G_{j+1}}"
    },
    {
      "row": 3,
      "col": 2,
      "label": "F_{i-1} \\otimes G_{j}"
    },
    {
      "row": 3,
      "col": 3,
      "label": "{F_{i-1} \\otimes G_{j-1}}"
    },
    {
      "row": 3,
      "col": 4,
      "label": "\\cdots"
    },
    {
      "row": 3,
      "col": 5,
      "label": "{F_{i+1}\\otimes N}"
    },
    {
      "row": 4,
      "col": 1,
      "label": "\\vdots"
    },
    {
      "row": 4,
      "col": 2,
      "label": "\\vdots"
    },
    {
      "row": 4,
      "col": 3,
      "label": "\\vdots"
    },
    {
      "row": 4,
      "col": 5,
      "label": "\\vdots"
    },
    {
      "row": 5,
      "col": 0,
      "label": "\\cdots"
    },
    {
      "row": 5,
      "col": 1,
      "label": "{M\\otimes G_{j+1}}"
    },
    {
      "row": 5,
      "col": 2,
      "label": "{M\\otimes G_{j+1}}"
    },
    {
      "row": 5,
      "col": 3,
      "label": "{M\\otimes G_{j+1}}"
    },
    {
      "row": 5,
      "col": 4,
      "label": "\\cdots"
    },
    {
      "row": 5,
      "col": 5,
      "label": "{M\\otimes N}"
    }
  ],
  "arrows": [
    {
      "id": "a17",
      "from": {
        "row": 0,
        "col": 1
      },
      "to": {
        "row": 1,
        "col": 1
      },
      "head": "default",
      "lineStyle": "solid"
    },
    {
      "id": "a21",
      "from": {
        "row": 0,
        "col": 2
      },
      "to": {
        "row": 1,
        "col": 2
      },
      "head": "default",
      "lineStyle": "solid"
    },
    {
      "id": "a25",
      "from": {
        "row": 0,
        "col": 3
      },
      "to": {
        "row": 1,
        "col": 3
      },
      "head": "default",
      "lineStyle": "solid"
    },
    {
      "id": "a44",
      "from": {
        "row": 0,
        "col": 5
      },
      "to": {
        "row": 1,
        "col": 5
      },
      "head": "default",
      "lineStyle": "solid"
    },
    {
      "id": "a4",
      "from": {
        "row": 1,
        "col": 0
      },
      "to": {
        "row": 1,
        "col": 1
      },
      "head": "default",
      "lineStyle": "solid"
    },
    {
      "id": "a5",
      "from": {
        "row": 1,
        "col": 1
      },
      "to": {
        "row": 1,
        "col": 2
      },
      "head": "default",
      "lineStyle": "solid"
    },
    {
      "id": "a18",
      "from": {
        "row": 1,
        "col": 1
      },
      "to": {
        "row": 2,
        "col": 1
      },
      "head": "default",
      "lineStyle": "solid"
    },
    {
      "id": "a6",
      "from": {
        "row": 1,
        "col": 2
      },
      "to": {
        "row": 1,
        "col": 3
      },
      "head": "default",
      "lineStyle": "solid"
    },
    {
      "id": "a22",
      "from": {
        "row": 1,
        "col": 2
      },
      "to": {
        "row": 2,
        "col": 2
      },
      "head": "default",
      "lineStyle": "solid"
    },
    {
      "id": "a7",
      "from": {
        "row": 1,
        "col": 3
      },
      "to": {
        "row": 1,
        "col": 4
      },
      "head": "default",
      "lineStyle": "solid"
    },
    {
      "id": "a26",
      "from": {
        "row": 1,
        "col": 3
      },
      "to": {
        "row": 2,
        "col": 3
      },
      "head": "default",
      "lineStyle": "solid"
    },
    {
      "id": "a34",
      "from": {
        "row": 1,
        "col": 4
      },
      "to": {
        "row": 1,
        "col": 5
      },
      "head": "default",
      "lineStyle": "solid"
    },
    {
      "id": "a30",
      "from": {
        "row": 1,
        "col": 5
      },
      "to": {
        "row": 2,
        "col": 5
      },
      "head": "default",
      "lineStyle": "solid"
    },
    {
      "id": "a8",
      "from": {
        "row": 2,
        "col": 0
      },
      "to": {
        "row": 2,
        "col": 1
      },
      "head": "default",
      "lineStyle": "solid"
    },
    {
      "id": "a9",
      "from": {
        "row": 2,
        "col": 1
      },
      "to": {
        "row": 2,
        "col": 2
      },
      "head": "default",
      "lineStyle": "solid"
    },
    {
      "id": "a19",
      "from": {
        "row": 2,
        "col": 1
      },
      "to": {
        "row": 3,
        "col": 1
      },
      "head": "default",
      "lineStyle": "solid"
    },
    {
      "id": "a10",
      "from": {
        "row": 2,
        "col": 2
      },
      "to": {
        "row": 2,
        "col": 3
      },
      "head": "default",
      "lineStyle": "solid",
      "label": "{(-1)^i\\otimes\\psi_j}"
    },
    {
      "id": "a23",
      "from": {
        "row": 2,
        "col": 2
      },
      "to": {
        "row": 3,
        "col": 2
      },
      "head": "default",
      "lineStyle": "solid",
      "label": "{\\phi_i \\otimes 1}"
    },
    {
      "id": "a11",
      "from": {
        "row": 2,
        "col": 3
      },
      "to": {
        "row": 2,
        "col": 4
      },
      "head": "default",
      "lineStyle": "solid"
    },
    {
      "id": "a27",
      "from": {
        "row": 2,
        "col": 3
      },
      "to": {
        "row": 3,
        "col": 3
      },
      "head": "default",
      "lineStyle": "solid"
    },
    {
      "id": "a35",
      "from": {
        "row": 2,
        "col": 4
      },
      "to": {
        "row": 2,
        "col": 5
      },
      "head": "default",
      "lineStyle": "solid"
    },
    {
      "id": "a31",
      "from": {
        "row": 2,
        "col": 5
      },
      "to": {
        "row": 3,
        "col": 5
      },
      "head": "default",
      "lineStyle": "solid"
    },
    {
      "id": "a12",
      "from": {
        "row": 3,
        "col": 0
      },
      "to": {
        "row": 3,
        "col": 1
      },
      "head": "default",
      "lineStyle": "solid"
    },
    {
      "id": "a13",
      "from": {
        "row": 3,
        "col": 1
      },
      "to": {
        "row": 3,
        "col": 2
      },
      "head": "default",
      "lineStyle": "solid"
    },
    {
      "id": "a20",
      "from": {
        "row": 3,
        "col": 1
      },
      "to": {
        "row": 4,
        "col": 1
      },
      "head": "default",
      "lineStyle": "solid"
    },
    {
      "id": "a14",
      "from": {
        "row": 3,
        "col": 2
      },
      "to": {
        "row": 3,
        "col": 3
      },
      "head": "default",
      "lineStyle": "solid"
    },
    {
      "id": "a24",
      "from": {
        "row": 3,
        "col": 2
      },
      "to": {
        "row": 4,
        "col": 2
      },
      "head": "default",
      "lineStyle": "solid"
    },
    {
      "id": "a15",
      "from": {
        "row": 3,
        "col": 3
      },
      "to": {
        "row": 3,
        "col": 4
      },
      "head": "default",
      "lineStyle": "solid"
    },
    {
      "id": "a28",
      "from": {
        "row": 3,
        "col": 3
      },
      "to": {
        "row": 4,
        "col": 3
      },
      "head": "default",
      "lineStyle": "solid"
    },
    {
      "id": "a36",
      "from": {
        "row": 3,
        "col": 4
      },
      "to": {
        "row": 3,
        "col": 5
      },
      "head": "default",
      "lineStyle": "solid"
    },
    {
      "id": "a32",
      "from": {
        "row": 3,
        "col": 5
      },
      "to": {
        "row": 4,
        "col": 5
      },
      "head": "default",
      "lineStyle": "solid"
    },
    {
      "id": "a29",
      "from": {
        "row": 4,
        "col": 1
      },
      "to": {
        "row": 5,
        "col": 1
      },
      "head": "default",
      "lineStyle": "solid"
    },
    {
      "id": "a37",
      "from": {
        "row": 4,
        "col": 2
      },
      "to": {
        "row": 5,
        "col": 2
      },
      "head": "default",
      "lineStyle": "solid"
    },
    {
      "id": "a38",
      "from": {
        "row": 4,
        "col": 3
      },
      "to": {
        "row": 5,
        "col": 3
      },
      "head": "default",
      "lineStyle": "solid"
    },
    {
      "id": "a33",
      "from": {
        "row": 4,
        "col": 5
      },
      "to": {
        "row": 5,
        "col": 5
      },
      "head": "default",
      "lineStyle": "solid"
    },
    {
      "id": "a39",
      "from": {
        "row": 5,
        "col": 0
      },
      "to": {
        "row": 5,
        "col": 1
      },
      "head": "default",
      "lineStyle": "solid"
    },
    {
      "id": "a40",
      "from": {
        "row": 5,
        "col": 1
      },
      "to": {
        "row": 5,
        "col": 2
      },
      "head": "default",
      "lineStyle": "solid"
    },
    {
      "id": "a41",
      "from": {
        "row": 5,
        "col": 2
      },
      "to": {
        "row": 5,
        "col": 3
      },
      "head": "default",
      "lineStyle": "solid"
    },
    {
      "id": "a42",
      "from": {
        "row": 5,
        "col": 3
      },
      "to": {
        "row": 5,
        "col": 4
      },
      "head": "default",
      "lineStyle": "solid"
    },
    {
      "id": "a43",
      "from": {
        "row": 5,
        "col": 4
      },
      "to": {
        "row": 5,
        "col": 5
      },
      "head": "default",
      "lineStyle": "solid"
    }
  ]
}
```
Definimos ${} {}\text{tot}_{k}(\mathcal{F}, \mathcal{G}) = \bigoplus_{i+j=k}F_{i}\otimes G_{j} {}$ y ${}\partial_{k} = \phi_{i}\otimes 1 + (-1)^i \otimes \psi_{j}{}$. Es inmediato comprobar que ${}\partial_{k}\partial_{k+1} = 0{}$. Por tanto, ${}\text{tot}(\mathcal{F}\otimes \mathcal{G}){}$ es un [[complejo de cadenas]] al que llamaremos *complejo total* con diferencial ${}\partial{}$, al que llamaremos *diferencial total*.

Definimos el morfismo ${}\eta_{k} : \text{tot}_{k}(\mathcal{F},\mathcal{G}){}\to F_{k}\otimes N$ tal que
$$
\begin{align}
\eta_{k}(f\otimes g) = \begin{cases}
0 & \text{si } g\notin G_{0} \\
f\otimes \varepsilon(g) & \text{si } g \in G_{0}
\end{cases}
\end{align}
$$
Veamos que ${}\eta : \text{tot}(\mathcal{F},\mathcal{G})\to \mathcal{F}\otimes N{}$ es un [[morfismo de cadenas]]. Para ello veamos que el siguiente diagrama conmuta.
```cd
{
  "version": 1,
  "rows": 2,
  "cols": 7,
  "cells": [
    {
      "row": 0,
      "col": 0,
      "label": "\\cdots"
    },
    {
      "row": 0,
      "col": 1,
      "label": "\\text{tot}_{k+1}(\\mathcal{F}, \\mathcal{G})"
    },
    {
      "row": 0,
      "col": 2,
      "label": "\\text{tot}_{k}(\\mathcal{F}, \\mathcal{G})"
    },
    {
      "row": 0,
      "col": 3,
      "label": "\\text{tot}_{k-1}(\\mathcal{F}, \\mathcal{G})"
    },
    {
      "row": 0,
      "col": 4,
      "label": "\\cdots"
    },
    {
      "row": 0,
      "col": 5,
      "label": "\\text{tot}_{0}(\\mathcal{F}, \\mathcal{G})"
    },
    {
      "row": 0,
      "col": 6,
      "label": "0"
    },
    {
      "row": 1,
      "col": 0,
      "label": "\\cdots"
    },
    {
      "row": 1,
      "col": 1,
      "label": "{F_{k+1}\\otimes N}"
    },
    {
      "row": 1,
      "col": 2,
      "label": "{F_{k}\\otimes N}"
    },
    {
      "row": 1,
      "col": 3,
      "label": "{F_{k-1}\\otimes N}"
    },
    {
      "row": 1,
      "col": 4,
      "label": "\\cdots"
    },
    {
      "row": 1,
      "col": 5,
      "label": "{F_{0}\\otimes N}"
    },
    {
      "row": 1,
      "col": 6,
      "label": "0"
    }
  ],
  "arrows": [
    {
      "id": "a1",
      "from": {
        "row": 0,
        "col": 0
      },
      "to": {
        "row": 0,
        "col": 1
      },
      "head": "default",
      "lineStyle": "solid"
    },
    {
      "id": "a2",
      "from": {
        "row": 0,
        "col": 1
      },
      "to": {
        "row": 0,
        "col": 2
      },
      "label": "\\partial_{k+1}",
      "head": "default",
      "lineStyle": "solid"
    },
    {
      "id": "a12",
      "from": {
        "row": 0,
        "col": 1
      },
      "to": {
        "row": 1,
        "col": 1
      },
      "label": "\\eta_{k+1}",
      "head": "default",
      "lineStyle": "solid"
    },
    {
      "id": "a3",
      "from": {
        "row": 0,
        "col": 2
      },
      "to": {
        "row": 0,
        "col": 3
      },
      "label": "\\partial_k",
      "head": "default",
      "lineStyle": "solid"
    },
    {
      "id": "a13",
      "from": {
        "row": 0,
        "col": 2
      },
      "to": {
        "row": 1,
        "col": 2
      },
      "label": "\\eta_k",
      "head": "default",
      "lineStyle": "solid"
    },
    {
      "id": "a4",
      "from": {
        "row": 0,
        "col": 3
      },
      "to": {
        "row": 0,
        "col": 4
      },
      "label": "\\partial_{k-1}",
      "head": "default",
      "lineStyle": "solid"
    },
    {
      "id": "a14",
      "from": {
        "row": 0,
        "col": 3
      },
      "to": {
        "row": 1,
        "col": 3
      },
      "label": "\\eta_{k-1}",
      "head": "default",
      "lineStyle": "solid"
    },
    {
      "id": "a5",
      "from": {
        "row": 0,
        "col": 4
      },
      "to": {
        "row": 0,
        "col": 5
      },
      "label": "\\partial_1",
      "head": "default",
      "lineStyle": "solid"
    },
    {
      "id": "a6",
      "from": {
        "row": 0,
        "col": 5
      },
      "to": {
        "row": 0,
        "col": 6
      },
      "head": "default",
      "lineStyle": "solid"
    },
    {
      "id": "a15",
      "from": {
        "row": 0,
        "col": 5
      },
      "to": {
        "row": 1,
        "col": 5
      },
      "label": "\\eta_0",
      "head": "default",
      "lineStyle": "solid"
    },
    {
      "id": "a7",
      "from": {
        "row": 1,
        "col": 0
      },
      "to": {
        "row": 1,
        "col": 1
      },
      "head": "default",
      "lineStyle": "solid"
    },
    {
      "id": "a8",
      "from": {
        "row": 1,
        "col": 1
      },
      "to": {
        "row": 1,
        "col": 2
      },
      "label": "{\\phi_{k+1} \\otimes 1}",
      "head": "default",
      "lineStyle": "solid"
    },
    {
      "id": "a9",
      "from": {
        "row": 1,
        "col": 2
      },
      "to": {
        "row": 1,
        "col": 3
      },
      "label": "{\\phi_k \\otimes 1}",
      "head": "default",
      "lineStyle": "solid"
    },
    {
      "id": "a10",
      "from": {
        "row": 1,
        "col": 3
      },
      "to": {
        "row": 1,
        "col": 4
      },
      "label": "{\\phi_{k-1} \\otimes 1}",
      "head": "default",
      "lineStyle": "solid"
    },
    {
      "id": "a11",
      "from": {
        "row": 1,
        "col": 4
      },
      "to": {
        "row": 1,
        "col": 5
      },
      "label": "{\\phi_0 \\otimes 1}",
      "head": "default",
      "lineStyle": "solid"
    },
    {
      "id": "a16",
      "from": {
        "row": 1,
        "col": 5
      },
      "to": {
        "row": 1,
        "col": 6
      },
      "head": "default",
      "lineStyle": "solid"
    }
  ]
}
```
Sea ${}f\otimes g \in \text{tot}_{k}(\mathcal{F},\mathcal{G}){}$
- Si ${}f\otimes g \in F_{k}\otimes G_{0}{}$. Tenemos que:
$$
	\eta_{k-1}\partial_{k}(f\otimes g) = \eta_{k-1}(\phi_{k}(f)\otimes g + (-1)^{k}f\otimes\psi_{0}(g)) = \phi_{k}(f)\otimes \varepsilon(g) = (\phi_{k}\otimes 1) \circ \eta_{k}(f\otimes g).
$$
- Si ${}f\otimes g \in F_{k-1}\otimes G_{0}{}$ entonces trivialmente${}(\phi_{k}\otimes 1)\circ\eta_{k}(f\otimes g) = 0{}$, mientras que:
$$
\eta_{k-1}\partial_{k}(f\otimes g) = \eta_{k-1}\left(\phi_{k-1}(f)\otimes g + (-1)^{k-1}f\otimes \psi_{1}(g)\right) = (-1)^{k-1}f \otimes\varepsilon\psi_{1}(g) = 0
$$
- El resto de casos son triviales.
Por tanto ${}\eta{}$ es un [[morfismo de cadenas]]. Veamos ahora que ${}\eta{}$ es un [[cuasi-isomorfismo]], es decir, que induce un isomorfismo entre las homologías.
Claramente, ${}H_{n}(\eta){}$ está bien definido, pues ${}H_{n}{}$ es un [[functor]] para todo ${}n{}$. Falta comprobar que es un isomorfismo.
Probar con el lema de ensamblado acíclico y el cono del morfismo ${}\eta{}$.