Sea ${}\mathcal{A}{}$ una [[Categoría aditiva]] y ${}f\in \text{Hom}_{}(A, B){}$. El *conúcleo* de $f$, es un objeto $Q$, junto a un morfismo ${} {}q:B\to Q{}$ tal que ${} qf{}  = 0 {}$ y es universal con esa propiedad. Es decir, dado cualquier morfismo ${} {}q' : B \to Q'{} {}$ tal que ${} {}q'f = 0{} {}$, existe un único morfismo ${}u:Q \to Q'{}$ tal que el siguiente diagrama conmuta:
```cd
{
  "version": 1,
  "rows": 3,
  "cols": 3,
  "cells": [
    {
      "row": 0,
      "col": 1,
      "label": "B"
    },
    {
      "row": 1,
      "col": 0,
      "label": "A"
    },
    {
      "row": 1,
      "col": 1,
      "label": "Q"
    },
    {
      "row": 2,
      "col": 2,
      "label": "Q'"
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
        "col": 1
      },
      "head": "default",
      "lineStyle": "solid",
      "id": "a8",
      "label": "q",
      "labelPosition": "right"
    },
    {
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
      "id": "a11",
      "label": "q'"
    },
    {
      "from": {
        "row": 1,
        "col": 0
      },
      "to": {
        "row": 0,
        "col": 1
      },
      "head": "default",
      "lineStyle": "solid",
      "id": "a7",
      "label": "f"
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
      "id": "a9",
      "label": "0"
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
      "id": "a10",
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
      "id": "a12",
      "label": "\\exists! u",
      "labelOffset": {
        "x": -1.4954427083333333,
        "y": 0.2955729166666667
      }
    }
  ]
}
```
Es el objeto dual del [[Núcleo]].