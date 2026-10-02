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
#### 1. ${}H_{n}(g \circ f) = H_{n}(g) \circ H_{n}(f), \; \forall f:A \to B,\; g:B\to C{}$
