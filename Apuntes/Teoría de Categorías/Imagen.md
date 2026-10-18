Sea ${}\mathcal{A}{}$ una [[Categoría aditiva]] y ${}f\in \text{Hom}_{}(A, B){}$. La imagen de $f$, es un objeto $\text{Im}f$, junto a un [[Monomorfismo]] ${} {}m:\text{Im}f\to B{}$ cumpliendo la siguiente propiedad universal:
1. Existe un [[Epimorfismo]] ${}e: A \to \text{Im}f{}$ tal que ${}f = me{}$.
2. Para todo objeto ${}I{}$ con un epimorfismo ${}e' : A \to I{}$ y monomorfismo ${}m' : I \to B{}$  tales que ${}f = m'e'{}$ existe un único morfismo ${}v : \text{Im}f \to I{}$ tal que el siguiente diagrama conmuta:

```cd
{
  "version": 1,
  "rows": 4,
  "cols": 3,
  "cells": [
    {
      "row": 0,
      "col": 0,
      "label": "A"
    },
    {
      "row": 0,
      "col": 2,
      "label": "B"
    },
    {
      "row": 1,
      "col": 1,
      "label": "\\text{Im} f"
    },
    {
      "row": 3,
      "col": 1,
      "label": "I"
    }
  ],
  "arrows": [
    {
      "id": "a33",
      "from": {
        "row": 0,
        "col": 0
      },
      "to": {
        "row": 0,
        "col": 2
      },
      "label": "f",
      "head": "default",
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
        "col": 1
      },
      "label": "e",
      "head": "epi",
      "lineStyle": "solid"
    },
    {
      "id": "a36",
      "from": {
        "row": 0,
        "col": 0
      },
      "to": {
        "row": 3,
        "col": 1
      },
      "label": "e'",
      "head": "epi",
      "lineStyle": "solid",
      "curve": -0.5
    },
    {
      "id": "a35",
      "from": {
        "row": 1,
        "col": 1
      },
      "to": {
        "row": 0,
        "col": 2
      },
      "label": "m",
      "head": "hook",
      "lineStyle": "solid"
    },
    {
      "id": "a38",
      "from": {
        "row": 1,
        "col": 1
      },
      "to": {
        "row": 3,
        "col": 1
      },
      "label": "\\exists! v",
      "head": "default",
      "lineStyle": "dashed",
      "labelOffset": {
        "x": -1.2348090277777777,
        "y": -0.009114583333333334
      }
    },
    {
      "id": "a37",
      "from": {
        "row": 3,
        "col": 1
      },
      "to": {
        "row": 0,
        "col": 2
      },
      "label": "m'",
      "head": "hook",
      "lineStyle": "solid",
      "curve": -0.5
    }
  ]
}
```
