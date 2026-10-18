# Morfismos de cadenas
Sean C y D dos [[Complejo de cadenas|complejos de cadenas]]. Un morfismo ${}u:C\to D{}$ de complejos de cadenas es una familia ${}\{ u_{n} : C_{n} \to D_{n}\}_{n \in \mathbb{Z}}{}$ de morfismos tal que el siguiente diagrama conmuta:
```cd
{
  "version": 1,
  "rows": 2,
  "cols": 5,
  "cells": [
    {
      "row": 0,
      "col": 0,
      "label": "\\cdots"
    },
    {
      "row": 0,
      "col": 1,
      "label": "C_{n+1}"
    },
    {
      "row": 0,
      "col": 2,
      "label": "C_n"
    },
    {
      "row": 0,
      "col": 3,
      "label": "C_{n-1}"
    },
    {
      "row": 0,
      "col": 4,
      "label": "\\dots"
    },
    {
      "row": 1,
      "col": 0,
      "label": "\\cdots"
    },
    {
      "row": 1,
      "col": 1,
      "label": "D_{n+1}"
    },
    {
      "row": 1,
      "col": 2,
      "label": "D_n"
    },
    {
      "row": 1,
      "col": 3,
      "label": "D_{n-1}"
    },
    {
      "row": 1,
      "col": 4,
      "label": "\\dots"
    }
  ],
  "arrows": [
    {
      "id": "a13",
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
      "id": "a14",
      "from": {
        "row": 0,
        "col": 1
      },
      "to": {
        "row": 0,
        "col": 2
      },
      "label": "d_{n+1}",
      "labelPosition": "above",
      "head": "default",
      "lineStyle": "solid"
    },
    {
      "id": "a23",
      "from": {
        "row": 0,
        "col": 1
      },
      "to": {
        "row": 1,
        "col": 1
      },
      "label": "u_{n+1}",
      "head": "default",
      "lineStyle": "solid"
    },
    {
      "id": "a15",
      "from": {
        "row": 0,
        "col": 2
      },
      "to": {
        "row": 0,
        "col": 3
      },
      "label": "d_n",
      "head": "default",
      "lineStyle": "solid"
    },
    {
      "id": "a22",
      "from": {
        "row": 0,
        "col": 2
      },
      "to": {
        "row": 1,
        "col": 2
      },
      "label": "u_n",
      "head": "default",
      "lineStyle": "solid"
    },
    {
      "id": "a16",
      "from": {
        "row": 0,
        "col": 3
      },
      "to": {
        "row": 0,
        "col": 4
      },
      "head": "default",
      "lineStyle": "solid"
    },
    {
      "id": "a21",
      "from": {
        "row": 0,
        "col": 3
      },
      "to": {
        "row": 1,
        "col": 3
      },
      "label": "u_{n-1}",
      "head": "default",
      "lineStyle": "solid"
    },
    {
      "id": "a17",
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
      "id": "a18",
      "from": {
        "row": 1,
        "col": 1
      },
      "to": {
        "row": 1,
        "col": 2
      },
      "label": "\\delta_{n+1}",
      "labelPosition": "below",
      "head": "default",
      "lineStyle": "solid"
    },
    {
      "id": "a19",
      "from": {
        "row": 1,
        "col": 2
      },
      "to": {
        "row": 1,
        "col": 3
      },
      "label": "\\delta_n",
      "labelPosition": "below",
      "head": "default",
      "lineStyle": "solid"
    },
    {
      "id": "a20",
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
    }
  ]
}
```
## Proposición
Fijada una [[Categoría abeliana]] ${}\mathcal{A}{}$,  la clase de [[Complejo de cadenas|complejos de cadenas]] junto a los morfismos de cadenas es una [[Categoría abeliana]], denotada ${}\text{Ch}(\mathcal{A}){}$.
### Demostración
#### ${}\text{Ch}(\mathcal{A}){}$ es una [[Categoría]].
Sean ${}A, B, C,D$ complejos de cadenas y ${}f:A \to B{}$, ${}g:B\to C{}$ y ${}h : C \to D{}$ morfismos de cadenas. Como ${}\mathcal{A}{}$ es una [[Categoría abeliana]],  notemos que ${}\forall n \in \mathbb{Z}{}$, existen las composiciones, ${}h(gf) = (hg)f{}$, ${}\exists 1_{C_{n}} : C_{n}\to C_{n}{}$ y ${}1_{C_{n}} \circ g_{n} = g_{n} \circ 1_{B_{n}}{}$. Por tanto:
- La composición de dos morfismos de cadenas ${}v \circ u := \{ v_{n}\circ u_{n} \}_{n \in \mathbb{Z}}{}$ está bien definida y es asociativa.
- Para todo [[Complejo de cadenas]] ${}C{}$, existe el morfismo identidad ${}1_{C}:=\{ 1_{C_{n}} \}_{n\in \mathbb{Z}}{}$  y estos morfismos identidad cumplen las leyes de identidad.
Por tanto ${}\text{Ch}(\mathcal{A}){}$ es una [[Categoría]].

#### ${}\text{Ch}(\mathcal{A}){}$ es [[Categoría preaditiva|preaditiva]].
Análogamente, como ${}\mathcal{A}{}$ es abeliana, en concreto es aditiva, y para todo ${}n \in \mathbb{Z}{}$ se cumple que si:
```cd
{
  "version": 1,
  "rows": 1,
  "cols": 4,
  "cells": [
    {
      "row": 0,
      "col": 0,
      "label": "A_n"
    },
    {
      "row": 0,
      "col": 1,
      "label": "B_n"
    },
    {
      "row": 0,
      "col": 2,
      "label": "C_n"
    },
    {
      "row": 0,
      "col": 3,
      "label": "D_n"
    }
  ],
  "arrows": [
    {
      "id": "a8",
      "from": {
        "row": 0,
        "col": 0
      },
      "to": {
        "row": 0,
        "col": 1
      },
      "label": "f_n"
    },
    {
      "id": "a10",
      "from": {
        "row": 0,
        "col": 1
      },
      "to": {
        "row": 0,
        "col": 2
      },
      "label": "g'_n",
      "labelPosition": "below"
    },
    {
      "id": "a9",
      "from": {
        "row": 0,
        "col": 1
      },
      "to": {
        "row": 0,
        "col": 2
      },
      "label": "g_n",
      "labelPosition": "above"
    },
    {
      "id": "a11",
      "from": {
        "row": 0,
        "col": 2
      },
      "to": {
        "row": 0,
        "col": 3
      },
      "label": "h_n"
    }
  ]
}
```
entonces ${}h_{n}(g_{n} + g'_{n})f_{n}{}$. Por tanto, definiendo la suma de morfismos de cadenas ${}u+v := \{ u_{n}+v_{n} \}_{n\in \mathbb{Z}}{}$, tenemos inmediatamente que ${}\text{Hom}_{\text{Ch}(\mathcal{A})}(A, B){}$ es un grupo abeliano para complejos ${}A, B{}$ cualesquiera y la composición distribuye con la suma. Por tanto es una [[Categoría preaditiva]].
#### $\text{Ch}(\mathcal{A})$ es [[Categoría aditiva|aditiva]]
Es inmediato ver que el morfismo de cadenas trivial ${}0{}$ es al mismo tiempo un [[objeto inicial]] y [[objeto terminal|terminal]].
Sean ${}A,B,P\in\text{Ch}(\mathcal{A}){}$ y morfismos de cadenas ${}f:P\to A{}$ y ${}g:P\to B{}$.
Definimos ${}A\times B{}$ como:
```cd
{
  "version": 1,
  "rows": 2,
  "cols": 6,
  "cells": [
    {
      "row": 1,
      "col": 0,
      "label": "A\\times B:"
    },
    {
      "row": 1,
      "col": 1,
      "label": "\\cdots"
    },
    {
      "row": 1,
      "col": 2,
      "label": "A_{n+1} \\times B_{n+1}"
    },
    {
      "row": 1,
      "col": 3,
      "label": "A_n \\times B_n"
    },
    {
      "row": 1,
      "col": 4,
      "label": "A_{n-1} \\times B_{n-1}"
    },
    {
      "row": 1,
      "col": 5,
      "label": "\\cdots"
    }
  ],
  "arrows": [
    {
      "id": "a39",
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
      "id": "a40",
      "from": {
        "row": 1,
        "col": 2
      },
      "to": {
        "row": 1,
        "col": 3
      },
      "label": "d_{n+1}",
      "head": "default",
      "lineStyle": "solid"
    },
    {
      "id": "a41",
      "from": {
        "row": 1,
        "col": 3
      },
      "to": {
        "row": 1,
        "col": 4
      },
      "label": "d_n ",
      "head": "default",
      "lineStyle": "solid"
    },
    {
      "id": "a42",
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
    }
  ]
}
```
Donde para cada ${}n\in \mathbb{Z}{}$, ${}d_{n}{}$ es el morfismo definido de forma única mediante la propiedad universal del [[producto]] en el siguiente diagrama:
```cd
{
  "version": 1,
  "rows": 3,
  "cols": 3,
  "cells": [
    {
      "row": 1,
      "col": 0,
      "label": "A_n"
    },
    {
      "row": 1,
      "col": 1,
      "label": "A_n \\times B_n"
    },
    {
      "row": 1,
      "col": 2,
      "label": "B_n"
    },
    {
      "row": 2,
      "col": 0,
      "label": "A_{n-1}"
    },
    {
      "row": 2,
      "col": 1,
      "label": "A_{n-1} \\times B_{n-1}"
    },
    {
      "row": 2,
      "col": 2,
      "label": "B_{n-1}"
    }
  ],
  "arrows": [
    {
      "from": {
        "row": 1,
        "col": 0
      },
      "to": {
        "row": 2,
        "col": 0
      },
      "head": "default",
      "lineStyle": "solid",
      "id": "a44",
      "label": "\\delta_n"
    },
    {
      "from": {
        "row": 1,
        "col": 1
      },
      "to": {
        "row": 1,
        "col": 0
      },
      "head": "default",
      "lineStyle": "solid",
      "id": "a43",
      "label": "p_{A;n}",
      "labelPosition": "above"
    },
    {
      "from": {
        "row": 1,
        "col": 1
      },
      "to": {
        "row": 1,
        "col": 2
      },
      "head": "default",
      "lineStyle": "solid",
      "id": "a47",
      "label": "p_{B;n}",
      "labelPosition": "above"
    },
    {
      "from": {
        "row": 1,
        "col": 1
      },
      "to": {
        "row": 2,
        "col": 1
      },
      "head": "default",
      "lineStyle": "dashed",
      "id": "a49",
      "label": "\\exists! d_n"
    },
    {
      "from": {
        "row": 1,
        "col": 2
      },
      "to": {
        "row": 2,
        "col": 2
      },
      "head": "default",
      "lineStyle": "solid",
      "id": "a48",
      "label": "\\partial_n"
    },
    {
      "from": {
        "row": 2,
        "col": 1
      },
      "to": {
        "row": 2,
        "col": 0
      },
      "head": "default",
      "lineStyle": "solid",
      "id": "a45",
      "label": "p_{A;n-1}",
      "labelPosition": "below"
    },
    {
      "from": {
        "row": 2,
        "col": 1
      },
      "to": {
        "row": 2,
        "col": 2
      },
      "head": "default",
      "lineStyle": "solid",
      "id": "a46",
      "label": "p_{B;n-1}",
      "labelPosition": "below"
    }
  ]
}
```
**Nota: Dichos productos y proyecciones existen porque ${}\mathcal{A}{}$ es abeliana.**
Notemos ahora que, debido a la propiedad universal del [[producto]], para cada ${}n \in \mathbb{Z}{}$ tenemos:
```cd
{
  "version": 1,
  "rows": 2,
  "cols": 3,
  "cells": [
    {
      "row": 0,
      "col": 1,
      "label": "P_n"
    },
    {
      "row": 1,
      "col": 0,
      "label": "A_n"
    },
    {
      "row": 1,
      "col": 1,
      "label": "A_n \\times B_n"
    },
    {
      "row": 1,
      "col": 2,
      "label": "B_n"
    }
  ],
  "arrows": [
    {
      "id": "a50",
      "from": {
        "row": 0,
        "col": 1
      },
      "to": {
        "row": 1,
        "col": 0
      },
      "label": "f_n",
      "labelPosition": "above",
      "head": "default",
      "lineStyle": "solid"
    },
    {
      "id": "a54",
      "from": {
        "row": 0,
        "col": 1
      },
      "to": {
        "row": 1,
        "col": 1
      },
      "label": "\\exists! h_n",
      "head": "default",
      "lineStyle": "dashed"
    },
    {
      "id": "a51",
      "from": {
        "row": 0,
        "col": 1
      },
      "to": {
        "row": 1,
        "col": 2
      },
      "label": "g_n",
      "head": "default",
      "lineStyle": "solid"
    },
    {
      "id": "a52",
      "from": {
        "row": 1,
        "col": 1
      },
      "to": {
        "row": 1,
        "col": 0
      },
      "label": "p_{A;n}",
      "head": "default",
      "lineStyle": "solid"
    },
    {
      "id": "a53",
      "from": {
        "row": 1,
        "col": 1
      },
      "to": {
        "row": 1,
        "col": 2
      },
      "label": "p_{B;n}",
      "head": "default",
      "lineStyle": "solid",
      "labelPosition": "below"
    }
  ]
}
```
Por tanto, tenemos determinado un único morfismo de cadenas ${}h := \{ h_{n} \}_{n\in \mathbb{Z}}{}$ que hace que el siguiente diagrama conmute:
```cd
{
  "version": 1,
  "rows": 2,
  "cols": 3,
  "cells": [
    {
      "row": 0,
      "col": 1,
      "label": "P"
    },
    {
      "row": 1,
      "col": 0,
      "label": "A"
    },
    {
      "row": 1,
      "col": 1,
      "label": "A\\times B"
    },
    {
      "row": 1,
      "col": 2,
      "label": "B"
    }
  ],
  "arrows": [
    {
      "from": {
        "row": 0,
        "col": 1
      },
      "to": {
        "row": 1,
        "col": 0
      },
      "head": "default",
      "lineStyle": "solid",
      "id": "a55",
      "label": "f",
      "labelPosition": "above"
    },
    {
      "from": {
        "row": 0,
        "col": 1
      },
      "to": {
        "row": 1,
        "col": 1
      },
      "head": "default",
      "lineStyle": "dashed",
      "id": "a59",
      "label": "\\exists!h"
    },
    {
      "from": {
        "row": 0,
        "col": 1
      },
      "to": {
        "row": 1,
        "col": 2
      },
      "head": "default",
      "lineStyle": "solid",
      "id": "a56",
      "label": "g"
    },
    {
      "from": {
        "row": 1,
        "col": 1
      },
      "to": {
        "row": 1,
        "col": 0
      },
      "head": "default",
      "lineStyle": "solid",
      "id": "a58",
      "label": "p_A"
    },
    {
      "from": {
        "row": 1,
        "col": 1
      },
      "to": {
        "row": 1,
        "col": 2
      },
      "head": "default",
      "lineStyle": "solid",
      "id": "a57",
      "label": "p_B",
      "labelPosition": "below"
    }
  ]
}
```
Luego ${}A\times B{}$ es precisamente el [[producto]] de ${}A{}$ y ${}B{}$.
Por tanto ${}\text{Ch}(\mathcal{A}){}$ es una [[Categoría aditiva]].
#### ${}\text{Ch}(\mathcal{A}){}$ es [[Categoría abeliana|abeliana]].
##### 1. Todo morfismo tiene [[Núcleo]] y [[Conúcleo]].
Sean ${}C, D{}$ complejos de cadenas y ${}u:C \to D{}$ un morfismo de cadenas
Como ${}\mathcal{A}{}$ es abeliana, para todo ${}n \in \mathbb{Z}{}$ tenemos el siguiente diagrama conmutativo:
```cd
{
  "version": 1,
  "rows": 4,
  "cols": 2,
  "cells": [
    {
      "row": 0,
      "col": 0,
      "label": "\\text{Ker} \\, u_{n}"
    },
    {
      "row": 0,
      "col": 1,
      "label": "\\text{Ker} \\, u_{n-1}"
    },
    {
      "row": 1,
      "col": 0,
      "label": "C_n"
    },
    {
      "row": 1,
      "col": 1,
      "label": "C_{n-1}"
    },
    {
      "row": 2,
      "col": 0,
      "label": "D_n"
    },
    {
      "row": 2,
      "col": 1,
      "label": "D_{n-1}"
    },
    {
      "row": 3,
      "col": 0,
      "label": "\\text{Coker} \\,u_{n}"
    },
    {
      "row": 3,
      "col": 1,
      "label": "\\text{Coker} \\,u_{n-1}"
    }
  ],
  "arrows": [
    {
      "id": "a3",
      "from": {
        "row": 0,
        "col": 0
      },
      "to": {
        "row": 1,
        "col": 0
      },
      "label": "k_n",
      "head": "hook"
    },
    {
      "id": "a4",
      "from": {
        "row": 0,
        "col": 1
      },
      "to": {
        "row": 1,
        "col": 1
      },
      "label": "k_{n-1}",
      "head": "hook"
    },
    {
      "id": "a5",
      "from": {
        "row": 1,
        "col": 0
      },
      "to": {
        "row": 1,
        "col": 1
      },
      "label": "d_n"
    },
    {
      "id": "a6",
      "from": {
        "row": 1,
        "col": 0
      },
      "to": {
        "row": 2,
        "col": 0
      },
      "label": "u_n"
    },
    {
      "id": "a7",
      "from": {
        "row": 1,
        "col": 1
      },
      "to": {
        "row": 2,
        "col": 1
      },
      "label": "u_{n-1}"
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
      "label": "\\delta_n"
    },
    {
      "id": "a9",
      "from": {
        "row": 2,
        "col": 0
      },
      "to": {
        "row": 3,
        "col": 0
      },
      "label": "q_n",
      "head": "epi"
    },
    {
      "id": "a10",
      "from": {
        "row": 2,
        "col": 1
      },
      "to": {
        "row": 3,
        "col": 1
      },
      "label": "q_{n-1}",
      "head": "epi"
    }
  ]
}
```
Notemos que ${}u_{n-1}(d_{n}k_{n}) = (u_{n-1}d_{n})k_{n} = (\delta_{n}u_{n})k_{n} = \delta_{n}(u_{n}k_{n}) = \delta_{n}\, 0{} = 0$. Por tanto, por la propiedad universal del [[Núcleo]], ${}\exists! \varphi_{n}:\text{Ker}\,u_{n}\to \text{Ker}\,u_{n-1}{}$. Además, ${}(q_{n-1}\delta_{n})u_{n}= q_{n-1}(\delta_{n}u_{n}) = q_{n-1}(u_{n-1}d_{n}) = (q_{n-1}u_{n-1})d_{n }=0d_{n} = 0{}$. Por tanto,  por la propiedad universal del [[Conúcleo]], ${}\exists! \psi_{n}:\text{Coker}\,u_{n}\to \text{Coker}\,u_{n-1}{}$.
Por tanto tenemos el siguiente diagrama conmutativo:
```cd
{
  "version": 1,
  "rows": 4,
  "cols": 6,
  "cells": [
    {
      "row": 0,
      "col": 0,
      "label": "\\text{Ker}\\, u: "
    },
    {
      "row": 0,
      "col": 1,
      "label": "\\cdots"
    },
    {
      "row": 0,
      "col": 2,
      "label": "\\text{Ker } u_{n+1}"
    },
    {
      "row": 0,
      "col": 3,
      "label": "\\text{Ker } u_{n}"
    },
    {
      "row": 0,
      "col": 4,
      "label": "\\text{Ker } u_{n-1}"
    },
    {
      "row": 0,
      "col": 5,
      "label": "\\cdots"
    },
    {
      "row": 1,
      "col": 0,
      "label": "C: "
    },
    {
      "row": 1,
      "col": 1,
      "label": "\\cdots"
    },
    {
      "row": 1,
      "col": 2,
      "label": "C_{n+1}"
    },
    {
      "row": 1,
      "col": 3,
      "label": "C_{n}"
    },
    {
      "row": 1,
      "col": 4,
      "label": "C_{n-1}"
    },
    {
      "row": 1,
      "col": 5,
      "label": "\\cdots"
    },
    {
      "row": 2,
      "col": 0,
      "label": "D: "
    },
    {
      "row": 2,
      "col": 1,
      "label": "\\cdots"
    },
    {
      "row": 2,
      "col": 2,
      "label": "D_{n+1}"
    },
    {
      "row": 2,
      "col": 3,
      "label": "D_{n}"
    },
    {
      "row": 2,
      "col": 4,
      "label": "D_{n-1}"
    },
    {
      "row": 2,
      "col": 5,
      "label": "\\cdots"
    },
    {
      "row": 3,
      "col": 0,
      "label": "\\text{Coker } u:"
    },
    {
      "row": 3,
      "col": 1,
      "label": "\\cdots"
    },
    {
      "row": 3,
      "col": 2,
      "label": "\\text{Coker } u_{n+1}"
    },
    {
      "row": 3,
      "col": 3,
      "label": "\\text{Coker } u_{n}"
    },
    {
      "row": 3,
      "col": 4,
      "label": "\\text{Coker } u_{n-1}"
    },
    {
      "row": 3,
      "col": 5,
      "label": "\\cdots"
    }
  ],
  "arrows": [
    {
      "id": "a27",
      "from": {
        "row": 0,
        "col": 0
      },
      "to": {
        "row": 1,
        "col": 0
      },
      "label": "k",
      "head": "hook",
      "lineStyle": "solid"
    },
    {
      "id": "a11",
      "from": {
        "row": 0,
        "col": 1
      },
      "to": {
        "row": 0,
        "col": 2
      },
      "head": "default",
      "lineStyle": "solid"
    },
    {
      "id": "a12",
      "from": {
        "row": 0,
        "col": 2
      },
      "to": {
        "row": 0,
        "col": 3
      },
      "label": "\\varphi_{n+1}",
      "head": "default",
      "lineStyle": "solid"
    },
    {
      "id": "a30",
      "from": {
        "row": 0,
        "col": 2
      },
      "to": {
        "row": 1,
        "col": 2
      },
      "label": "k_{n+1}",
      "head": "hook",
      "lineStyle": "solid"
    },
    {
      "id": "a13",
      "from": {
        "row": 0,
        "col": 3
      },
      "to": {
        "row": 0,
        "col": 4
      },
      "label": "\\varphi_n",
      "head": "default",
      "lineStyle": "solid"
    },
    {
      "id": "a33",
      "from": {
        "row": 0,
        "col": 3
      },
      "to": {
        "row": 1,
        "col": 3
      },
      "label": "k_n",
      "head": "hook",
      "lineStyle": "solid"
    },
    {
      "id": "a14",
      "from": {
        "row": 0,
        "col": 4
      },
      "to": {
        "row": 0,
        "col": 5
      },
      "head": "default",
      "lineStyle": "solid"
    },
    {
      "id": "a36",
      "from": {
        "row": 0,
        "col": 4
      },
      "to": {
        "row": 1,
        "col": 4
      },
      "label": "k_{n-1}",
      "head": "hook",
      "lineStyle": "solid"
    },
    {
      "id": "a28",
      "from": {
        "row": 1,
        "col": 0
      },
      "to": {
        "row": 2,
        "col": 0
      },
      "label": "u",
      "head": "default",
      "lineStyle": "solid"
    },
    {
      "id": "a15",
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
      "id": "a16",
      "from": {
        "row": 1,
        "col": 2
      },
      "to": {
        "row": 1,
        "col": 3
      },
      "label": "d_{n+1}",
      "head": "default",
      "lineStyle": "solid"
    },
    {
      "id": "a31",
      "from": {
        "row": 1,
        "col": 2
      },
      "to": {
        "row": 2,
        "col": 2
      },
      "label": "u_{n+1}",
      "head": "default",
      "lineStyle": "solid"
    },
    {
      "id": "a17",
      "from": {
        "row": 1,
        "col": 3
      },
      "to": {
        "row": 1,
        "col": 4
      },
      "label": "d_n",
      "head": "default",
      "lineStyle": "solid"
    },
    {
      "id": "a34",
      "from": {
        "row": 1,
        "col": 3
      },
      "to": {
        "row": 2,
        "col": 3
      },
      "label": "u_n",
      "head": "default",
      "lineStyle": "solid"
    },
    {
      "id": "a18",
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
      "id": "a37",
      "from": {
        "row": 1,
        "col": 4
      },
      "to": {
        "row": 2,
        "col": 4
      },
      "label": "u_{n-1}",
      "head": "default",
      "lineStyle": "solid"
    },
    {
      "id": "a29",
      "from": {
        "row": 2,
        "col": 0
      },
      "to": {
        "row": 3,
        "col": 0
      },
      "label": "q",
      "head": "epi",
      "lineStyle": "solid"
    },
    {
      "id": "a19",
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
      "id": "a20",
      "from": {
        "row": 2,
        "col": 2
      },
      "to": {
        "row": 2,
        "col": 3
      },
      "label": "\\delta_{n+1}",
      "head": "default",
      "lineStyle": "solid"
    },
    {
      "id": "a32",
      "from": {
        "row": 2,
        "col": 2
      },
      "to": {
        "row": 3,
        "col": 2
      },
      "label": "q_{n+1}",
      "head": "epi",
      "lineStyle": "solid"
    },
    {
      "id": "a21",
      "from": {
        "row": 2,
        "col": 3
      },
      "to": {
        "row": 2,
        "col": 4
      },
      "label": "\\delta_n",
      "head": "default",
      "lineStyle": "solid"
    },
    {
      "id": "a35",
      "from": {
        "row": 2,
        "col": 3
      },
      "to": {
        "row": 3,
        "col": 3
      },
      "label": "q_n",
      "head": "epi",
      "lineStyle": "solid"
    },
    {
      "id": "a22",
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
      "id": "a38",
      "from": {
        "row": 2,
        "col": 4
      },
      "to": {
        "row": 3,
        "col": 4
      },
      "label": "q_{n-1}",
      "head": "epi",
      "lineStyle": "solid"
    },
    {
      "id": "a23",
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
      "id": "a24",
      "from": {
        "row": 3,
        "col": 2
      },
      "to": {
        "row": 3,
        "col": 3
      },
      "label": "\\psi_{n+1}",
      "head": "default",
      "lineStyle": "solid"
    },
    {
      "id": "a25",
      "from": {
        "row": 3,
        "col": 3
      },
      "to": {
        "row": 3,
        "col": 4
      },
      "label": "\\psi_n",
      "head": "default",
      "lineStyle": "solid"
    },
    {
      "id": "a26",
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
    }
  ]
}
```
Comprobemos ahora que, efectivamente, ${}\text{Ker}\,u{}$ y ${}\text{Coker}\,u{}$ son complejos de cadenas y son el [[Núcleo]] y el [[Conúcleo]] de ${}u{}$,  respectivamente. En efecto, notemos que 
$$
k_{n-1} \varphi_{n}\varphi_{{n+1}} = d_{n}d_{n+1}k_{n+1} = 0\,k_{n+1} = 0
$$
Además, como ${}k_{n-1}{}$ es mono, concluimos que ${}\varphi_{n}\varphi_{n+1} = 0{}$, luego ${}\text{Ker}\,u{}$ es un [[Complejo de cadenas]]. Análogamente,
$$
\psi_{n}\psi_{n+1}q_{n+1} = q_{n-1}\delta_{n}\delta_{n+1} = q_{n-1}\,0 = 0
$$
Como ${}q_{n+1}{}$ es epi, concluimos que ${}\psi_{n}\psi_{n+1} = 0{}$ y por tanto ${}\text{Coker}\,u{}$ es un [[Complejo de cadenas]].
Supongamos ahora que existen complejos de cadenas ${}K, Q{}$ con morfismos de cadenas ${}k':K\to C{}$ y ${}q' :D \to Q{}$ tales que ${}uk' = 0{}$ y ${}q'u =0{}$. Notemos que, como para cada ${}n\in \mathbb{Z}{}$ ${}u_{n}k'_{n} = 0{}$ y ${}q'_{n}u_{n} = 0{}$, por las propiedades universales del [[Núcleo]] y el [[Conúcleo]] existirán ${}\iota_{n} : K_{n}\to \text{Ker}\,u_{n}{}$ y ${}\pi_{n} : \text{Coker}\,u_{n}\to Q_{n}{}$ *únicos* tales que ${}k_{n}\iota_{n} = k'_{n}{}$ y ${}\pi_{n}q_{n} = q'_{n}{}$. Luego los morfismos de cadenas ${}\iota := \{ \iota_{n} \}_{n\in \mathbb{Z}}, \; \pi:=\{ \pi_{n} \}_{n\in \mathbb{Z}}{}$ quedan definidos de forma única y cumplen que ${}k\iota = k'{}$ y ${}\pi q = q'{}$. Por tanto son el [[Núcleo]] y el [[Conúcleo]] de ${}u{}$.
##### 2. Todo [[Monomorfismo]] de ${}\text{Ch}(\mathcal{A}){}$ es el [[Núcleo]] de su [[Conúcleo]]
Sean ${}A, B{}$ complejos de cadenas y ${}f:A\to B{}$ un [[Monomorfismo]]. Veamos que dado ${}n \in \mathbb{Z}{}$, ${}f_{n} : A_{n}\to B_{n}{}$ también es un [[Monomorfismo]]. Sea ${}g_{n} : A'_{n} \to A_{n}{}$ un morfismo tal que ${}f_{n}g_{n} = 0{}$. Para ello, definimos el [[Complejo de cadenas]] ${}C{}$ y el morfismo de cadenas ${}g:C \to A{}$, de tal forma que si ${}k = n{}$, entonces ${}g_{k} = g_{n}{}$ y ${}g_{k}= 0{}$ en otro caso.
Por construcción, tenemos que ${}fg = 0{}$. Como ${}f{}$ es mónico, ${}g = 0{}$. En particular ${}g_{n} = 0{}$, luego ${}f_{n}{}$ también es un [[Monomorfismo]].

Ahora bien, notemos que dado un [[Complejo de cadenas]] ${}C{}$ y un morfismo de cadenas ${}g : C \to B{}$ tal que ${}qg = 0{}$, donde ${}q : B \to \text{Coker}\,f{}$. Como ${}\mathcal{A}{}$ es una [[Categoría abeliana]], tenemos que ${}f_{n}{}$ es el [[Núcleo]] de su [[Conúcleo]] ${}\forall n \in \mathbb{Z}{}$ y por tanto existirá un único morfismo ${}u_{n} : C_{n} \to A_{n}{}$ tal que el siguiente diagrama conmute:
```cd
{
  "version": 1,
  "rows": 3,
  "cols": 3,
  "cells": [
    {
      "row": 0,
      "col": 1,
      "label": "B_n"
    },
    {
      "row": 1,
      "col": 1,
      "label": "A_n"
    },
    {
      "row": 1,
      "col": 2,
      "label": "\\text{Coker }f"
    },
    {
      "row": 2,
      "col": 0,
      "label": "C_n"
    }
  ],
  "arrows": [
    {
      "id": "a62",
      "from": {
        "row": 0,
        "col": 1
      },
      "to": {
        "row": 1,
        "col": 2
      },
      "label": "q_n",
      "head": "default",
      "lineStyle": "solid"
    },
    {
      "id": "a60",
      "from": {
        "row": 1,
        "col": 1
      },
      "to": {
        "row": 0,
        "col": 1
      },
      "label": "f_n",
      "head": "default",
      "lineStyle": "solid"
    },
    {
      "id": "a61",
      "from": {
        "row": 1,
        "col": 1
      },
      "to": {
        "row": 1,
        "col": 2
      },
      "label": "0",
      "head": "default",
      "lineStyle": "solid"
    },
    {
      "id": "a63",
      "from": {
        "row": 2,
        "col": 0
      },
      "to": {
        "row": 0,
        "col": 1
      },
      "label": "g_n",
      "head": "default",
      "lineStyle": "solid",
      "curve": 0.5
    },
    {
      "id": "a65",
      "from": {
        "row": 2,
        "col": 0
      },
      "to": {
        "row": 1,
        "col": 1
      },
      "label": "\\exists!u_n",
      "head": "default",
      "lineStyle": "dashed",
      "labelOffset": {
        "x": 0.98046875,
        "y": 0.5360243055555556
      }
    },
    {
      "id": "a64",
      "from": {
        "row": 2,
        "col": 0
      },
      "to": {
        "row": 1,
        "col": 2
      },
      "label": "0",
      "head": "default",
      "lineStyle": "solid",
      "curve": -0.5
    }
  ]
}
```
Por tanto, tenemos que existe un único morfismo de cadenas ${}u := \{ u_{n} \}_{n\in \mathbb{Z}}:C \to A{}$ tal que ${}fu = g{}$, es decir, ${}f{}$ es el [[Núcleo]] de ${}q{}$.
##### 3. Todo [[Epimorfismo]] de ${}\text{Ch}(\mathcal{A}){}$ es el [[Conúcleo]] de su [[Núcleo]]
Sean ${}A, B{}$ complejos de cadenas y ${}f:A\to B{}$ un [[Epimorfismo]]. Veamos que dado ${}n \in \mathbb{Z}{}$, ${}f_{n} : A_{n}\to B_{n}{}$ también es un [[Epimorfismo]]. Sea ${}g_{n} : B_{n} \to B'_{n}{}$ un morfismo tal que ${}g_{n}f_{n} = 0{}$. Para ello, definimos el [[Complejo de cadenas]] ${}C{}$ y el morfismo de cadenas ${} {}g:B \to C{} {}$, de tal forma que si ${}k = n{}$, entonces ${}g_{k} = g_{n}{}$ y ${}g_{k}= 0{}$ en otro caso.
Por construcción, tenemos que ${} gf= 0{} {}$. Como ${}f{}$ es epi, ${}g = 0{}$. En particular ${}g_{n} = 0{}$, luego ${}f_{n}{}$ también es un [[Epimorfismo]].

Ahora bien, notemos que dado un [[Complejo de cadenas]] ${}C{}$ y un morfismo de cadenas ${} {}g : A \to C{} {}$ tal que ${} gk= 0{}$, donde ${} k: \text{Ker}\,f \to A {}$. Como ${}\mathcal{A}{}$ es una [[Categoría abeliana]], tenemos que ${}f_{n}{}$ es el [[Conúcleo]] de su [[Núcleo]] ${}\forall n \in \mathbb{Z}{}$ y por tanto existirá un único morfismo ${}u_{n} : B_{n} \to C_{n}{}$ tal que el siguiente diagrama conmute:
```cd
{
  "version": 1,
  "rows": 3,
  "cols": 3,
  "cells": [
    {
      "row": 0,
      "col": 1,
      "label": "A_n"
    },
    {
      "row": 1,
      "col": 0,
      "label": "\\text{Ker }f_n"
    },
    {
      "row": 1,
      "col": 1,
      "label": "B_n"
    },
    {
      "row": 2,
      "col": 2,
      "label": "C_n"
    }
  ],
  "arrows": [
    {
      "id": "a67",
      "from": {
        "row": 0,
        "col": 1
      },
      "to": {
        "row": 1,
        "col": 1
      },
      "label": "f",
      "head": "default",
      "lineStyle": "solid"
    },
    {
      "id": "a69",
      "from": {
        "row": 0,
        "col": 1
      },
      "to": {
        "row": 2,
        "col": 2
      },
      "head": "default",
      "lineStyle": "solid",
      "label": "g_n",
      "curve": 0.5
    },
    {
      "id": "a68",
      "from": {
        "row": 1,
        "col": 0
      },
      "to": {
        "row": 0,
        "col": 1
      },
      "label": "k_n",
      "head": "default",
      "lineStyle": "solid"
    },
    {
      "id": "a66",
      "from": {
        "row": 1,
        "col": 0
      },
      "to": {
        "row": 1,
        "col": 1
      },
      "label": "0",
      "head": "default",
      "lineStyle": "solid"
    },
    {
      "from": {
        "row": 1,
        "col": 0
      },
      "to": {
        "row": 2,
        "col": 2
      },
      "head": "default",
      "lineStyle": "solid",
      "id": "a70",
      "curve": -0.45,
      "label": "0",
      "labelPosition": "below"
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
      "lineStyle": "dashed",
      "id": "a71",
      "label": "\\exists!u_n",
      "labelOffset": {
        "x": 0.11263020833333333,
        "y": -1.0598958333333333
      },
      "labelPosition": "below"
    }
  ]
}
```

Por tanto, tenemos que existe un único morfismo de cadenas ${} {}u := \{ u_{n} \}_{n\in \mathbb{Z}}:B \to C{} {}$ tal que ${} {}uf = g{} {}$, es decir, ${}f{}$ es el [[Conúcleo]] de ${}q{}$.

Por tanto, tenemos que ${}\text{Ch}(\mathcal{A}){}$ es una [[Categoría abeliana]].