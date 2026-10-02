Una [[Categoría|categoría]] $\mathcal{A}$ es una *categoría preaditiva* si todo conjunto $\text{Hom}_\mathcal{A}(A,B)$ en $\mathcal{A}$ es un grupo abeliano de tal forma que la composición distribuye con la suma. Es decir, dado el siguiente diagrama:

```cd
{
  "version": 1,
  "rows": 1,
  "cols": 4,
  "cells": [
    {
      "row": 0,
      "col": 0,
      "label": "A"
    },
    {
      "row": 0,
      "col": 1,
      "label": "B"
    },
    {
      "row": 0,
      "col": 2,
      "label": "C"
    },
    {
      "row": 0,
      "col": 3,
      "label": "D"
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
      "label": "f",
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
      "label": "g'",
      "labelPosition": "below",
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
        "row": 0,
        "col": 2
      },
      "label": "g",
      "head": "default",
      "lineStyle": "solid"
    },
    {
      "id": "a4",
      "from": {
        "row": 0,
        "col": 2
      },
      "to": {
        "row": 0,
        "col": 3
      },
      "label": "h",
      "head": "default",
      "lineStyle": "solid"
    }
  ]
}
```
tenemos que $h(g+g')f = hgf + hg'f$.