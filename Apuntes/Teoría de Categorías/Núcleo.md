Sea ${}\mathcal{A}{}$ una [[Categoría aditiva]] y ${} {}f\in \text{Hom}_{}(A, B){} {}$. El *núcleo* de $f$, es un objeto $K$, junto a un morfismo ${} {}k:K\to {}A$ tal que $fk = 0$ y es universal con esa propiedad. Es decir, dado cualquier morfismo ${}k' : K' \to A{}$ tal que ${}fk' = 0{}$, existe un único morfismo ${}u:K' \to K{}$ tal que el siguiente diagrama conmuta:
```cd
{
  "version": 1,
  "rows": 3,
  "cols": 3,
  "cells": [
    {
      "row": 0,
      "col": 1,
      "label": "A"
    },
    {
      "row": 1,
      "col": 1,
      "label": "K"
    },
    {
      "row": 1,
      "col": 2,
      "label": "B"
    },
    {
      "row": 2,
      "col": 0,
      "label": "K'"
    }
  ],
  "arrows": [
    {
      "id": "a1",
      "from": {
        "row": 0,
        "col": 1
      },
      "to": {
        "row": 1,
        "col": 2
      },
      "label": "f",
      "head": "default",
      "lineStyle": "solid"
    },
    {
      "id": "a3",
      "from": {
        "row": 1,
        "col": 1
      },
      "to": {
        "row": 0,
        "col": 1
      },
      "label": "k",
      "labelPosition": "right",
      "head": "default",
      "lineStyle": "solid"
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
      "label": "0",
      "labelPosition": "above",
      "head": "default",
      "lineStyle": "solid"
    },
    {
      "id": "a4",
      "from": {
        "row": 2,
        "col": 0
      },
      "to": {
        "row": 0,
        "col": 1
      },
      "label": "k'",
      "head": "default",
      "lineStyle": "solid",
      "curve": 0.25
    },
    {
      "id": "a6",
      "from": {
        "row": 2,
        "col": 0
      },
      "to": {
        "row": 1,
        "col": 1
      },
      "head": "default",
      "lineStyle": "dashed",
      "label": "\\exists! u",
      "labelPosition": "above",
      "labelOffset": {
        "x": 1.0503472222222223,
        "y": 0.6154513888888888
      }
    },
    {
      "id": "a5",
      "from": {
        "row": 2,
        "col": 0
      },
      "to": {
        "row": 1,
        "col": 2
      },
      "head": "default",
      "lineStyle": "solid",
      "label": "0",
      "labelPosition": "right",
      "labelOffset": {
        "x": 0.7447916666666666,
        "y": 0.20182291666666666
      },
      "curve": -0.2
    }
  ]
}
```
