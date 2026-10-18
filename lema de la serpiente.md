# Lema de la serpiente
Sea ${}\mathcal{A}{}$ una [[categoría abeliana]] y ${}A,A', B,B', C, C' \in \mathcal{A}{}$ tales que el siguiente diagrama conmuta y sus filas son exactas:
```cd
{
  "version": 1,
  "rows": 2,
  "cols": 5,
  "cells": [
    {
      "row": 0,
      "col": 1,
      "label": "A"
    },
    {
      "row": 0,
      "col": 2,
      "label": "B"
    },
    {
      "row": 0,
      "col": 3,
      "label": "C"
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
      "label": "A'"
    },
    {
      "row": 1,
      "col": 2,
      "label": "B'"
    },
    {
      "row": 1,
      "col": 3,
      "label": "C'"
    }
  ],
  "arrows": [
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
      "head": "default",
      "lineStyle": "solid",
      "label": "f"
    },
    {
      "id": "a16",
      "from": {
        "row": 0,
        "col": 1
      },
      "to": {
        "row": 1,
        "col": 1
      },
      "label": "a",
      "head": "default",
      "lineStyle": "solid"
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
      "head": "default",
      "lineStyle": "solid",
      "label": "g"
    },
    {
      "id": "a17",
      "from": {
        "row": 0,
        "col": 2
      },
      "to": {
        "row": 1,
        "col": 2
      },
      "label": "b",
      "head": "default",
      "lineStyle": "solid"
    },
    {
      "id": "a12",
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
      "id": "a18",
      "from": {
        "row": 0,
        "col": 3
      },
      "to": {
        "row": 1,
        "col": 3
      },
      "label": "c",
      "head": "default",
      "lineStyle": "solid"
    },
    {
      "id": "a13",
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
      "id": "a14",
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
      "label": "f'"
    },
    {
      "id": "a15",
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
      "label": "g'"
    }
  ]
}
```
Entonces existe un morfismo ${}\partial :\text{Ker}\,h\to \text{Coker}\,f{}$ tal que la siguiente sucesión es exacta:
$$
\text{Ker}\, f\to \text{Ker}\, a\to \text{Ker}\, b\to \text{Ker}\, c \overset{\partial}\to  \text{Coker}\, a\to \text{Coker}\, b \to \text{Coker}\, c\to \text{Coker}\, g'
$$
## Demostración
**TODO**