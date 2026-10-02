# Complejo de cadenas
Sea ${}\mathcal{A}{}$ una [[categoría abeliana]]. Un complejo de cadenas de ${}\mathcal{A}{}$, ${}C{}$, es una familia ${}\{C_{n}\}_{n \in \mathbb{Z}}{}$ de objetos de ${}\mathcal{A}{}$, junto a una familia de morfismos, ${}\{ d_{n} : C_{n} \to C_{n-1} \}_{n \in \mathbb{Z}}{}$ tales que ${}d_{n}\circ d_{n+1} = 0{}$. Esta última propiedad es equivalente a decir que, ${}\forall n \in \mathbb{Z}{}$ existe un único [[monomorfismo]], ${}\varphi_{n}:\text{Im}\,d_{n+1}\to \text{Ker}\,d_{n}{}$. En efecto, notemos que para todo  ${}n \in \mathbb{Z}{}$ tenemos el siguiente diagrama conmutativo:
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
      "id": "a2",
      "from": {
        "row": 0,
        "col": 1
      },
      "to": {
        "row": 1,
        "col": 2
      },
      "label": "m_{n+1}",
      "head": "hook"
    },
    {
      "id": "a3",
      "from": {
        "row": 0,
        "col": 3
      },
      "to": {
        "row": 1,
        "col": 2
      },
      "label": "k_n",
      "head": "hook",
      "labelPosition": "above"
    },
    {
      "id": "a7",
      "from": {
        "row": 0,
        "col": 3
      },
      "to": {
        "row": 1,
        "col": 4
      },
      "label": "0",
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
        "row": 0,
        "col": 1
      },
      "label": "e_{n+1}",
      "head": "epi"
    },
    {
      "id": "a5",
      "from": {
        "row": 1,
        "col": 0
      },
      "to": {
        "row": 1,
        "col": 2
      },
      "label": "d_{n+1}"
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
      "label": "d_n"
    }
  ]
}
```
Como ${}d_{n}d_{n+1} = d_{n}m_{n+1}e_{n+1} = 0{}$, como ${}e_{n+1}{}$ es [[Epimorfismo|epi]], tenemos que ${}d_{n}m_{n+1} = 0{}$. Por la propiedad universal del [[núcleo]] y el hecho de que todo [[núcleo]] es [[Monomorfismo|mónico]] tenemos que existirá un único [[monomorfismo]] ${}\varphi_{n} : \text{Im}\,d_{n+1} \to \text{Ker}\,d_{n}{}$  que  mantenga la conmutatividad del diagrama anterior.

Si no da lugar a confusión, no mencionaremos la [[categoría abeliana]] subyacente.