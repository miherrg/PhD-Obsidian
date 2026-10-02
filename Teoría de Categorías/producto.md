Dada una categoría ${}\mathcal{A}{}$ y dos objetos $A, B \in \mathcal{A}$, el *producto de A y B* es un objeto, ${}A \times B \in \mathcal{A}{}$, junto a dos morfismos, ${}p_{1}\in \text{Hom}_{}(A\times B, A), \; p_{2}\in \text{Hom}_{}(A\times B, B){}$, que es **universal** con respecto a estos morfismos. Es decir, para todo objeto ${}P\in \mathcal{A}{}$, con morfismos ${}f_{1}:P \to A{}$ y $f_{2}:P \to B$, existe un único morfismo ${}f:P \to A \times B{}$ de tal forma que el siguiente diagrama conmuta.
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
      "label": "A \\times B"
    },
    {
      "row": 1,
      "col": 2,
      "label": "B"
    }
  ],
  "arrows": [
    {
      "id": "a5",
      "from": {
        "row": 0,
        "col": 1
      },
      "to": {
        "row": 1,
        "col": 0
      },
      "label": "f_1",
      "labelPosition": "above",
      "head": "default",
      "lineStyle": "solid"
    },
    {
      "id": "a9",
      "from": {
        "row": 0,
        "col": 1
      },
      "to": {
        "row": 1,
        "col": 1
      },
      "label": "\\exists! f",
      "labelPosition": "left",
      "head": "default",
      "lineStyle": "dashed"
    },
    {
      "id": "a6",
      "from": {
        "row": 0,
        "col": 1
      },
      "to": {
        "row": 1,
        "col": 2
      },
      "label": "f_2",
      "head": "default",
      "lineStyle": "solid"
    },
    {
      "id": "a7",
      "from": {
        "row": 1,
        "col": 1
      },
      "to": {
        "row": 1,
        "col": 0
      },
      "label": "p_1",
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
      "label": "p_2",
      "head": "default",
      "lineStyle": "solid",
      "labelPosition": "below"
    }
  ]
}
```
**EL PRODUCTO NO TIENE POR QUÉ EXISTIR, PERO SI EXISTE, ES ÚNICO.**