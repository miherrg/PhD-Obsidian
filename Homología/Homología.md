# Homología de cadenas
Sea ${}\mathcal{A}{}$ una [[Categoría abeliana]], y ${}C{}$ un [[complejo de cadenas]]. Para cada ${}n \in \mathbb{Z}{}$ tenemos el siguiente diagrama conmutativo:
```cd
{
  "version": 1,
  "rows": 2,
  "cols": 5,
  "cells": [
    {
      "row": 0,
      "col": 1,
      "label": "\\text{Im}\\,d_{n+1}"
    },
    {
      "row": 0,
      "col": 3,
      "label": "\\text{Ker}\\, d_n"
    },
    {
      "row": 1,
      "col": 0,
      "label": "C_{n+1}"
    },
    {
      "row": 1,
      "col": 2,
      "label": "C_n"
    },
    {
      "row": 1,
      "col": 4,
      "label": "C_{n-1}"
    }
  ],
  "arrows": [
    {
      "id": "a12",
      "from": {
        "row": 0,
        "col": 1
      },
      "to": {
        "row": 0,
        "col": 3
      },
      "label": "\\varphi_n",
      "head": "hook",
      "lineStyle": "solid"
    },
    {
      "id": "a8",
      "from": {
        "row": 0,
        "col": 1
      },
      "to": {
        "row": 1,
        "col": 2
      },
      "label": "m_{n+1}",
      "head": "hook",
      "lineStyle": "solid"
    },
    {
      "id": "a11",
      "from": {
        "row": 0,
        "col": 3
      },
      "to": {
        "row": 1,
        "col": 2
      },
      "label": "k_n",
      "labelPosition": "above",
      "head": "hook",
      "lineStyle": "solid",
      "labelOffset": {
        "x": 0.4817708333333333,
        "y": -0.16710069444444445
      }
    },
    {
      "id": "a7",
      "from": {
        "row": 1,
        "col": 0
      },
      "to": {
        "row": 0,
        "col": 1
      },
      "label": "e_{n+1}",
      "head": "epi",
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
        "col": 2
      },
      "label": "d_{n+1}",
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
        "col": 4
      },
      "label": "d_n",
      "head": "default",
      "lineStyle": "solid"
    }
  ]
}
```
Definimos la *n-ésima* homología de ${}C{}$ como
$$
H_{n}(C) = \text{Coker}\, \varphi_{n}
$$
## Proposición
${}H_{n}(-){}$ es un [[functor]] de ${}\text{Ch}(\mathcal{A}){}$ en ${}\mathcal{A}{}$.
### Demostración
Por definición, ${}H_{n}(C) \in \mathcal{A}{}$. Veamos que dado un [[morfismo de cadenas]] ${}u: C \to D{}$, existe un morfismo ${}H_{n}(u) : H_{n}(C) \to H_{n}(D){}$ que cumple los axiomas functoriales.
#### 1. Para todo ${}u : A \to B{}$, existe ${}H_{n}(u){}$.
Notemos que tenemos el siguiente diagrama conmutativo.
```cd
{
  "version": 1,
  "rows": 6,
  "cols": 3,
  "cells": [
    {
      "row": 0,
      "col": 1,
      "label": "H_n(A)"
    },
    {
      "row": 1,
      "col": 0,
      "label": "\\text{Im}\\, d_{n+1}"
    },
    {
      "row": 1,
      "col": 1,
      "label": "\\text{Ker}\\, d_n"
    },
    {
      "row": 2,
      "col": 0,
      "label": "A_{n+1}"
    },
    {
      "row": 2,
      "col": 1,
      "label": "A_n"
    },
    {
      "row": 2,
      "col": 2,
      "label": "A_{n-1}"
    },
    {
      "row": 3,
      "col": 0,
      "label": "B_{n+1}"
    },
    {
      "row": 3,
      "col": 1,
      "label": "B_n"
    },
    {
      "row": 3,
      "col": 2,
      "label": "B_{n-1}"
    },
    {
      "row": 4,
      "col": 0,
      "label": "\\text{Im}\\, \\delta_{n+1}"
    },
    {
      "row": 4,
      "col": 1,
      "label": "\\text{Ker}\\, \\delta_n"
    },
    {
      "row": 5,
      "col": 1,
      "label": "H_n(B)"
    }
  ],
  "arrows": [
    {
      "id": "a3",
      "from": {
        "row": 1,
        "col": 0
      },
      "to": {
        "row": 0,
        "col": 1
      },
      "label": "0",
      "head": "default",
      "lineStyle": "solid"
    },
    {
      "id": "a1",
      "from": {
        "row": 1,
        "col": 0
      },
      "to": {
        "row": 1,
        "col": 1
      },
      "label": "\\varphi_n",
      "head": "hook",
      "lineStyle": "solid"
    },
    {
      "id": "a13",
      "from": {
        "row": 1,
        "col": 0
      },
      "to": {
        "row": 2,
        "col": 1
      },
      "label": "m_{n+1}",
      "labelPosition": "left",
      "head": "hook",
      "lineStyle": "solid",
      "labelOffset": {
        "x": -1.6762152777777777,
        "y": 1.6059027777777777
      }
    },
    {
      "id": "a2",
      "from": {
        "row": 1,
        "col": 1
      },
      "to": {
        "row": 0,
        "col": 1
      },
      "label": "q_n",
      "head": "epi",
      "lineStyle": "solid"
    },
    {
      "id": "a11",
      "from": {
        "row": 1,
        "col": 1
      },
      "to": {
        "row": 2,
        "col": 1
      },
      "label": "k_n",
      "head": "hook",
      "lineStyle": "solid"
    },
    {
      "from": {
        "row": 1,
        "col": 1
      },
      "to": {
        "row": 2,
        "col": 2
      },
      "head": "default",
      "lineStyle": "solid",
      "id": "a20",
      "label": "0"
    },
    {
      "id": "a12",
      "from": {
        "row": 2,
        "col": 0
      },
      "to": {
        "row": 1,
        "col": 0
      },
      "label": "e_{n+1}",
      "head": "epi",
      "lineStyle": "solid"
    },
    {
      "id": "a4",
      "from": {
        "row": 2,
        "col": 0
      },
      "to": {
        "row": 2,
        "col": 1
      },
      "label": "d_{n+1}",
      "labelPosition": "below",
      "head": "default",
      "lineStyle": "solid"
    },
    {
      "id": "a14",
      "from": {
        "row": 2,
        "col": 0
      },
      "to": {
        "row": 3,
        "col": 0
      },
      "label": "u_{n+1}",
      "head": "default",
      "lineStyle": "solid"
    },
    {
      "id": "a5",
      "from": {
        "row": 2,
        "col": 1
      },
      "to": {
        "row": 2,
        "col": 2
      },
      "label": "d_n",
      "labelPosition": "below",
      "head": "default",
      "lineStyle": "solid"
    },
    {
      "id": "a15",
      "from": {
        "row": 2,
        "col": 1
      },
      "to": {
        "row": 3,
        "col": 1
      },
      "label": "u_n",
      "head": "default",
      "lineStyle": "solid"
    },
    {
      "id": "a16",
      "from": {
        "row": 2,
        "col": 2
      },
      "to": {
        "row": 3,
        "col": 2
      },
      "label": "u_{n-1}",
      "head": "default",
      "lineStyle": "solid"
    },
    {
      "id": "a6",
      "from": {
        "row": 3,
        "col": 0
      },
      "to": {
        "row": 3,
        "col": 1
      },
      "label": "\\delta_{n+1}",
      "head": "default",
      "lineStyle": "solid"
    },
    {
      "id": "a17",
      "from": {
        "row": 3,
        "col": 0
      },
      "to": {
        "row": 4,
        "col": 0
      },
      "label": "\\tilde e_{n+1}",
      "labelPosition": "right",
      "head": "epi",
      "lineStyle": "solid"
    },
    {
      "id": "a7",
      "from": {
        "row": 3,
        "col": 1
      },
      "to": {
        "row": 3,
        "col": 2
      },
      "label": "\\delta_n",
      "head": "default",
      "lineStyle": "solid"
    },
    {
      "id": "a18",
      "from": {
        "row": 4,
        "col": 0
      },
      "to": {
        "row": 3,
        "col": 1
      },
      "label": "\\tilde m_{n+1}",
      "head": "hook",
      "lineStyle": "solid",
      "labelOffset": {
        "x": -0.2769097222222222,
        "y": 0.65234375
      }
    },
    {
      "id": "a8",
      "from": {
        "row": 4,
        "col": 0
      },
      "to": {
        "row": 4,
        "col": 1
      },
      "label": "\\psi_n",
      "head": "hook",
      "lineStyle": "solid"
    },
    {
      "id": "a10",
      "from": {
        "row": 4,
        "col": 0
      },
      "to": {
        "row": 5,
        "col": 1
      },
      "label": "0",
      "head": "default",
      "lineStyle": "solid"
    },
    {
      "id": "a19",
      "from": {
        "row": 4,
        "col": 1
      },
      "to": {
        "row": 3,
        "col": 1
      },
      "label": "\\tilde k_n",
      "head": "hook",
      "lineStyle": "solid"
    },
    {
      "from": {
        "row": 4,
        "col": 1
      },
      "to": {
        "row": 3,
        "col": 2
      },
      "head": "default",
      "lineStyle": "solid",
      "id": "a21",
      "label": "0",
      "labelPosition": "right"
    },
    {
      "id": "a9",
      "from": {
        "row": 4,
        "col": 1
      },
      "to": {
        "row": 5,
        "col": 1
      },
      "label": "\\tilde q_n",
      "head": "epi",
      "lineStyle": "solid"
    }
  ]
}
```
Notemos que ${}\delta_{n} u_{n}k_{n} = u_{n-1}d_{n}k_{n} = u_{n-1}\, 0 = 0{}$. Por la propiedad universal del núcleo, ${}\exists!v_{n} : \text{Ker}\,d_{n}\to \text{Ker}\,\delta_{n}{}$ tal que ${}\tilde k_{n}v_{n} = u_{n}k_{n}{}$.
Además, como el diagrama es conmuativo, ${}\tilde q_{n}v_{n}\varphi_{n}e_{n+1}=0 \circ \tilde e_{n+1}u_{n+1} = 0{}$, como ${}e_{n+1}{}$ es [[epimorfismo]], tenemos que ${}\tilde q_{n}v_{n}\varphi_{n} = 0{}$. Por tanto, por la propiedad universal del conúcleo, ${}\exists!w_{n} : H_{n}(A) \to H_{n}(B){}$ tal que ${}w_{n}q_{n} = \tilde q_{n}v_{n}{}$.
#### 2. ${}H_{n}(g \circ f) = H_{n}(g) \circ H_{n}(f), \; \forall f:A \to B,\; g:B\to C{}$
