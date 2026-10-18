# Exactitud
Sea ${}\mathcal{A}{}$ una [[Categoría abeliana]]. Diremos que un [[Complejo de cadenas]], ${}C{}$ es *exacto* en ${}C_{n}{}$ si ${}\text{Im}\,d_{n+1} = \text{Ker}\,d_{n}{}$.

# Sucesión Exacta
Diremos que un [[complejo de cadenas]], ${}C{}$,  es una *sucesión exacta* si C es exacto en ${}C_{n}{}, \; \forall n \in \mathbb{Z}$.
## Proposición
Si C es una sucesión exacta, entonces ${}H_{n}(C) = 0, \; \forall n \in \mathbb{Z}{}$.
### Demostración
TODO
# Sucesión exacta corta
Una *sucesión exacta corta* es una sucesión exacta de la forma 
$$
\cdots \to 0 \to A \to B \to C \to 0 \to \cdots
$$
Normalmente se escribe solamente ${}0\to A \to B \to C \to 0{}$.
# Teorema: Sucesión exacta larga de [[homología|homologías]]
Sea ${}0 \to A \overset f \to B \overset g \to C \to 0{}$ una sucesión exacta corta. Entonces existen morfismos naturales ${}\partial_{n} : H_{n}(C)\to H_{n-1}(A){}$, llamados morfismos conexión, tales que
$$
\cdots \to H_{n+1}(C) \overset{\partial_{n+1}}{\to} H_{n}(A)\overset{f^*_{n}}{\to }H_{n}(B)\overset{g^*_{n}}{\to } H_{n}(C) \overset{\partial_{n}}{\to }H_{n-1}(A)\to \cdots
$$
es una sucesión exacta.
## Demostración
La sucesión exacta corta de [[Complejo de cadenas|complejos de cadenas]] nos da lugar al siguiente diagrama conmutativo cuyas filas sucesiones exactas cortas, ${}\forall n \in \mathbb{Z}{}$:
```cd
{
  "version": 1,
  "rows": 2,
  "cols": 5,
  "cells": [
    {
      "row": 0,
      "col": 0,
      "label": "0"
    },
    {
      "row": 0,
      "col": 1,
      "label": "A_n"
    },
    {
      "row": 0,
      "col": 2,
      "label": "B_n"
    },
    {
      "row": 0,
      "col": 3,
      "label": "C_n"
    },
    {
      "row": 0,
      "col": 4,
      "label": "0"
    },
    {
      "row": 1,
      "col": 0,
      "label": "0"
    },
    {
      "row": 1,
      "col": 1,
      "label": "A_{n-1}"
    },
    {
      "row": 1,
      "col": 2,
      "label": "B_{n-1}"
    },
    {
      "row": 1,
      "col": 3,
      "label": "C_{n-1}"
    },
    {
      "row": 1,
      "col": 4,
      "label": "0"
    }
  ],
  "arrows": [
    {
      "from": {
        "row": 0,
        "col": 0
      },
      "to": {
        "row": 0,
        "col": 1
      },
      "head": "default",
      "lineStyle": "solid",
      "id": "a1"
    },
    {
      "from": {
        "row": 0,
        "col": 1
      },
      "to": {
        "row": 0,
        "col": 2
      },
      "head": "default",
      "lineStyle": "solid",
      "id": "a2",
      "label": "f_n"
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
      "lineStyle": "solid",
      "id": "a9",
      "label": "d^A_n"
    },
    {
      "from": {
        "row": 0,
        "col": 2
      },
      "to": {
        "row": 0,
        "col": 3
      },
      "head": "default",
      "lineStyle": "solid",
      "id": "a3",
      "label": "g_n"
    },
    {
      "from": {
        "row": 0,
        "col": 2
      },
      "to": {
        "row": 1,
        "col": 2
      },
      "head": "default",
      "lineStyle": "solid",
      "id": "a10",
      "label": "d^B_n"
    },
    {
      "from": {
        "row": 0,
        "col": 3
      },
      "to": {
        "row": 0,
        "col": 4
      },
      "head": "default",
      "lineStyle": "solid",
      "id": "a4"
    },
    {
      "from": {
        "row": 0,
        "col": 3
      },
      "to": {
        "row": 1,
        "col": 3
      },
      "head": "default",
      "lineStyle": "solid",
      "id": "a11",
      "label": "d^C_n"
    },
    {
      "from": {
        "row": 1,
        "col": 0
      },
      "to": {
        "row": 1,
        "col": 1
      },
      "head": "default",
      "lineStyle": "solid",
      "id": "a5"
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
      "id": "a6",
      "label": "f_{n-1}"
    },
    {
      "from": {
        "row": 1,
        "col": 2
      },
      "to": {
        "row": 1,
        "col": 3
      },
      "head": "default",
      "lineStyle": "solid",
      "id": "a7",
      "label": "g_{n-1}"
    },
    {
      "from": {
        "row": 1,
        "col": 3
      },
      "to": {
        "row": 1,
        "col": 4
      },
      "head": "default",
      "lineStyle": "solid",
      "id": "a8"
    }
  ]
}
```
Por tanto, podemos aplicar el [[lema de la serpiente]] obteniendo la siguiente sucesión exacta ${} {}\forall n{} {}$:
$$
0 \to \text{Ker}\, d^A_{n} \to \text{Ker}\, d^B_{n} \to \text{Ker}\, d^C_{n} \to \text{Coker}\, d_{n}^A\to \text{Coker}\, d_{n}^B\to \text{Coker}\, d_{n}^C \to  0
$$
Ahora bien, consideremos el siguiente diagrama conmutativo:
```cd
{
  "version": 1,
  "rows": 3,
  "cols": 4,
  "cells": [
    {
      "row": 0,
      "col": 1,
      "label": "{\\text{Coker }d^A_{n+1}}"
    },
    {
      "row": 1,
      "col": 0,
      "label": "A_{n+1}"
    },
    {
      "row": 1,
      "col": 1,
      "label": "A_n"
    },
    {
      "row": 1,
      "col": 2,
      "label": "A_{n-1}"
    },
    {
      "row": 1,
      "col": 3,
      "label": "A_{n-2}"
    },
    {
      "row": 2,
      "col": 1,
      "label": "{\\text{Im }d^A_n}"
    },
    {
      "row": 2,
      "col": 2,
      "label": "{\\text{Ker }d^A_{n-1}}"
    }
  ],
  "arrows": [
    {
      "id": "a20",
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
      "id": "a12",
      "from": {
        "row": 1,
        "col": 0
      },
      "to": {
        "row": 1,
        "col": 1
      },
      "label": "d_{n+1}^A",
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
        "row": 0,
        "col": 1
      },
      "label": "q_{n+1}",
      "head": "epi",
      "lineStyle": "solid"
    },
    {
      "id": "a13",
      "from": {
        "row": 1,
        "col": 1
      },
      "to": {
        "row": 1,
        "col": 2
      },
      "label": "d_{n}^A",
      "head": "default",
      "lineStyle": "solid"
    },
    {
      "id": "a16",
      "from": {
        "row": 1,
        "col": 1
      },
      "to": {
        "row": 2,
        "col": 1
      },
      "label": "e_n",
      "head": "epi",
      "lineStyle": "solid"
    },
    {
      "id": "a14",
      "from": {
        "row": 1,
        "col": 2
      },
      "to": {
        "row": 1,
        "col": 3
      },
      "label": "d_{n-1}^A",
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
        "row": 1,
        "col": 2
      },
      "label": "m_n",
      "head": "hook",
      "lineStyle": "solid",
      "labelOffset": {
        "x": -0.1111111111111111,
        "y": 0.3333333333333333
      }
    },
    {
      "id": "a17",
      "from": {
        "row": 2,
        "col": 1
      },
      "to": {
        "row": 2,
        "col": 2
      },
      "label": "\\varphi_n",
      "head": "hook",
      "lineStyle": "solid"
    },
    {
      "id": "a18",
      "from": {
        "row": 2,
        "col": 2
      },
      "to": {
        "row": 1,
        "col": 2
      },
      "label": "k_{n-1}",
      "head": "hook",
      "lineStyle": "solid"
    },
    {
      "id": "a21",
      "from": {
        "row": 2,
        "col": 2
      },
      "to": {
        "row": 1,
        "col": 3
      },
      "label": "0",
      "labelPosition": "below",
      "head": "default",
      "lineStyle": "solid"
    }
  ]
}
```
Notemos que ${}k_{n-1}\varphi_{n}e_{n}d_{n+1}^A = d_{n}^Ad_{n-1}^A = 0{}$, pero ${}k_{n-1}{}$ es mónico, luego ${}\varphi_{n}e_{n}d_{n+1}^A = 0{}$. Por la propiedad universal del [[conúcleo]],  ${}{\exists!\psi^A_{n}:\text{Coker}\,d_{n+1}^A\to \text{Ker}\,d_{n-1}^A}{}$  tal que ${} {{}\psi_{n}q_{n+1} = \varphi_{n}e_{n}{}}$.
Repitiendo el razonamiento para ${}B, C{}$ obtenemos el siguiente diagrama conmutativo:
```cd
{
  "version": 1,
  "rows": 2,
  "cols": 5,
  "cells": [
    {
      "row": 0,
      "col": 1,
      "label": "\\text{Coker }d_{n+1}^A"
    },
    {
      "row": 0,
      "col": 2,
      "label": "\\text{Coker }d_{n+1}^B"
    },
    {
      "row": 0,
      "col": 3,
      "label": "\\text{Coker }d_{n+1}^C"
    },
    {
      "row": 0,
      "col": 4,
      "label": "0"
    },
    {
      "row": 1,
      "col": 0,
      "label": "0"
    },
    {
      "row": 1,
      "col": 1,
      "label": "\\text{Ker } d_{n-1}^A"
    },
    {
      "row": 1,
      "col": 2,
      "label": "\\text{Ker } d_{n-1}^B"
    },
    {
      "row": 1,
      "col": 3,
      "label": "\\text{Ker } d_{n-1}^C"
    }
  ],
  "arrows": [
    {
      "from": {
        "row": 0,
        "col": 1
      },
      "to": {
        "row": 0,
        "col": 2
      },
      "head": "default",
      "lineStyle": "solid",
      "id": "a25"
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
      "lineStyle": "solid",
      "id": "a28",
      "label": "\\psi^A_n"
    },
    {
      "from": {
        "row": 0,
        "col": 2
      },
      "to": {
        "row": 0,
        "col": 3
      },
      "head": "default",
      "lineStyle": "solid",
      "id": "a26"
    },
    {
      "from": {
        "row": 0,
        "col": 2
      },
      "to": {
        "row": 1,
        "col": 2
      },
      "head": "default",
      "lineStyle": "solid",
      "id": "a29",
      "label": "\\psi^B_n"
    },
    {
      "from": {
        "row": 0,
        "col": 3
      },
      "to": {
        "row": 0,
        "col": 4
      },
      "head": "default",
      "lineStyle": "solid",
      "id": "a27"
    },
    {
      "from": {
        "row": 0,
        "col": 3
      },
      "to": {
        "row": 1,
        "col": 3
      },
      "head": "default",
      "lineStyle": "solid",
      "id": "a30",
      "label": "\\psi^C_n"
    },
    {
      "from": {
        "row": 1,
        "col": 0
      },
      "to": {
        "row": 1,
        "col": 1
      },
      "head": "default",
      "lineStyle": "solid",
      "id": "a22"
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
      "id": "a23"
    },
    {
      "from": {
        "row": 1,
        "col": 2
      },
      "to": {
        "row": 1,
        "col": 3
      },
      "head": "default",
      "lineStyle": "solid",
      "id": "a24"
    }
  ]
}
```
Aplicando de nuevo el [[lema de la serpiente]], obtenemos la siguiente sucesión exacta:
$$
\text{Ker}\, \psi^A_{n} \to \text{Ker}\, \psi^B_{n} \to \text{Ker}\, \psi^C_{n} \to \text{Coker}\, \psi_{n}^A\to \text{Coker}\, \psi_{n}^B\to \text{Coker}\, \psi_{n}^C
$$
### ${}\text{Ker}\,\psi_{n}^\bullet = H_{n}(\bullet){}$
Hagámoslo para ${}A{}$ y el razonamiento para ${}B$ y ${}C{}$ es análogo. Consideremos el siguiente diagrama conmutativo.
```cd
{
  "version": 1,
  "rows": 2,
  "cols": 3,
  "cells": [
    {
      "row": 0,
      "col": 0,
      "label": "H_n(A)"
    },
    {
      "row": 0,
      "col": 1,
      "label": "\\text{Coker }d_{n+1}"
    },
    {
      "row": 0,
      "col": 2,
      "label": "\\text{Ker } \\phi_n"
    },
    {
      "row": 1,
      "col": 0,
      "label": "\\text{Im } d_n"
    },
    {
      "row": 1,
      "col": 1,
      "label": "\\text{Ker }d_{n-1}"
    }
  ],
  "arrows": [
    {
      "id": "a31",
      "from": {
        "row": 0,
        "col": 0
      },
      "to": {
        "row": 0,
        "col": 1
      },
      "label": "\\iota",
      "head": "hook",
      "lineStyle": "solid"
    },
    {
      "id": "a34",
      "from": {
        "row": 0,
        "col": 0
      },
      "to": {
        "row": 1,
        "col": 0
      },
      "label": "0",
      "head": "default",
      "lineStyle": "solid"
    },
    {
      "id": "a33",
      "from": {
        "row": 0,
        "col": 1
      },
      "to": {
        "row": 1,
        "col": 0
      },
      "label": "\\psi_n",
      "labelPosition": "right",
      "head": "epi",
      "lineStyle": "solid"
    },
    {
      "id": "a36",
      "from": {
        "row": 0,
        "col": 1
      },
      "to": {
        "row": 1,
        "col": 1
      },
      "label": "\\phi_n",
      "head": "default",
      "lineStyle": "solid"
    },
    {
      "id": "a32",
      "from": {
        "row": 0,
        "col": 2
      },
      "to": {
        "row": 0,
        "col": 1
      },
      "label": "\\iota'",
      "labelPosition": "above",
      "head": "hook",
      "lineStyle": "solid"
    },
    {
      "id": "a37",
      "from": {
        "row": 0,
        "col": 2
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
      "id": "a35",
      "from": {
        "row": 1,
        "col": 0
      },
      "to": {
        "row": 1,
        "col": 1
      },
      "label": "\\varphi_{n-1}",
      "labelPosition": "below",
      "head": "hook",
      "lineStyle": "solid"
    }
  ]
}
```
Tenemos que ${}\phi_{n}\iota = \varphi_{n-1}\psi_{n}\iota = \varphi_{n-1}0 = 0{}$, luego por la propiedad universal del [[núcleo]], ${}\exists!v : H_{n}(A)\to \text{Ker}\,\phi_{n}{}$ tal que ${}\iota' v = \iota{}$. Además ${}\varphi_{n-1}\psi_{n}\iota' = \phi_{n}\iota' = 0{}$. Como ${}\varphi_{n-1}{}$ es mono,  ${}\psi_{n}\iota' = 0{}$. Pero recordemos que ${}H_{n}(A) = \text{Ker}\,\psi_{n}{}$, luego por la propiedad universal del [[núcleo]], ${}\exists! u : \text{Ker}\,\phi_{n}\to H_{n}(A){}$ tal que ${}\iota u = \iota'{}$.
Ahora bien, notemos que ${}\iota' v u = \iota u = \iota' = \iota' \circ 1_{\text{Ker}\,\phi_{n}}{}$, pero ${}\iota'{}$ es mono; luego ${}vu = 1_{\text{Ker}\,\phi_{n}}{}$. De forma análoga, se demuestra que ${}uv = 1_{H_{n}(A)}{}$. Luego ${}v{}$ es un isomorfismo y, por tanto, ${}H_{n}(A) \cong \text{Ker}\,\phi_{n}{}$.
### ${}\text{Coker}\,\psi_{n}^\bullet = H_{n-1}(\bullet){}$
Hagámoslo para ${}A{}$ y el razonamiento para ${}B$ y ${}C{}$ es análogo. Consideremos el siguiente diagrama conmutativo.
```cd
{
  "version": 1,
  "rows": 2,
  "cols": 3,
  "cells": [
    {
      "row": 0,
      "col": 0,
      "label": "\\text{Im } d_n"
    },
    {
      "row": 0,
      "col": 1,
      "label": "\\text{Coker } d_{n+1}"
    },
    {
      "row": 1,
      "col": 0,
      "label": "H_{n-1}(A)"
    },
    {
      "row": 1,
      "col": 1,
      "label": "\\text{Ker } d_{n-1}"
    },
    {
      "row": 1,
      "col": 2,
      "label": "\\text{Coker }\\phi_n"
    }
  ],
  "arrows": [
    {
      "from": {
        "row": 0,
        "col": 0
      },
      "to": {
        "row": 1,
        "col": 0
      },
      "head": "default",
      "lineStyle": "solid",
      "id": "a9",
      "label": "0",
      "labelPosition": "right"
    },
    {
      "from": {
        "row": 0,
        "col": 0
      },
      "to": {
        "row": 1,
        "col": 1
      },
      "head": "hook",
      "lineStyle": "solid",
      "id": "a7",
      "label": "\\varphi_{n-1}",
      "labelOffset": {
        "x": 0.2222222222222222,
        "y": 0.5555555555555556
      }
    },
    {
      "from": {
        "row": 0,
        "col": 1
      },
      "to": {
        "row": 0,
        "col": 0
      },
      "head": "epi",
      "lineStyle": "solid",
      "id": "a6",
      "label": "\\psi_n",
      "labelPosition": "above"
    },
    {
      "id": "a1",
      "from": {
        "row": 0,
        "col": 1
      },
      "to": {
        "row": 1,
        "col": 1
      },
      "label": "\\phi_n",
      "head": "default",
      "lineStyle": "solid"
    },
    {
      "id": "a3",
      "from": {
        "row": 0,
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
      "from": {
        "row": 1,
        "col": 1
      },
      "to": {
        "row": 1,
        "col": 0
      },
      "head": "epi",
      "lineStyle": "solid",
      "id": "a8",
      "label": "\\epsilon"
    },
    {
      "id": "a2",
      "from": {
        "row": 1,
        "col": 1
      },
      "to": {
        "row": 1,
        "col": 2
      },
      "label": "\\epsilon'",
      "head": "epi",
      "lineStyle": "solid",
      "labelPosition": "below"
    }
  ]
}
```
Tenemos que ${}\epsilon' \varphi_{n-1}\psi_{n} = \epsilon' \phi_{n} = 0{}$. Como ${}\psi_{n}{}$ es epi, ${}\epsilon'\varphi_{n-1} = 0{}$. Como ${}H_{n-1}(A) = {\text{Coker}\,\varphi_{n-1}}{}$, por la propiedad universal del [[conúcleo]], ${}\exists!u : H_{n-1}(A)\to \text{Coker}\,\phi_{n}{}$ tal que ${}u\epsilon = \epsilon'{}$. De forma análoga, tenemos que ${}\epsilon\phi_{n} = \epsilon\varphi_{n-1}\psi_{n} = 0 \psi_{n} = 0{}$, luego por la propiedad universal del [[conúcleo]], ${}\exists!v:\text{Coker}\,\phi_{n}\to H_{n-1}(A){}$ tal que ${}v\epsilon' = \epsilon{}$. Ahora bien, notemos que ${}uv\epsilon' = u\epsilon = \epsilon'{}$, como ${}\epsilon'{}$ es epi, tenemos que ${}uv = 1_{\text{Coker}\,\phi_{n}}{}$. De forma análoga obtenemos que ${}vu = 1_{H_{n-1}(A)}{}$, luego ${}v{}$ es un isomorfismo y, por tanto, ${}H_{n-1}(A){}\cong \text{Coker}\,\phi_{n}$
### Construcción de la sucesión exacta larga.
Juntando estos dos últimos resultados con la sucesión exacta obtenida por el [[lema de la serpiente]], obtenemos  la siguiente sucesión exacta larga para cada ${}n\in \mathbb{Z}{}$:

$$
H_{n}(A)\overset{f_n*}\to  H_{n}(B)\overset{g_{n*}} \to H_{n}(C) \overset{\partial_{n}}{\to}H_{n-1}(A)\overset{f_{n-1*}}\to  H_{n-1}(B)\overset{g_{n-1*}} \to H_{n-1}(C)  
$$
Donde ${} {}f_{*}, g_{*}{} {}$ son los morfismos en [[homología]] de ${}f{}$ y ${}g{}$ respectivamente y ${}\partial_{n}{}$ es el morfismo conector dado por el lema de la serpiente.
Juntando todas las sucesiones, obtenemos la sucesión exacta larga deseada. 