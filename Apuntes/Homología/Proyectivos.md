# Objeto proyectivo
Un objeto ${}P{}$ en una [[Categoría abeliana]] ${}\mathcal{A}{}$ es *proyectivo* si dado un [[Epimorfismo]] ${}g : B  \to C{}$ y un morfismo ${}\gamma : P \to C{}$, existe ${}\beta : P \to B{}$ tal que ${}\gamma = g \beta{}$.
```cd
{
  "version": 1,
  "rows": 2,
  "cols": 2,
  "cells": [
    {
      "row": 0,
      "col": 1,
      "label": "P"
    },
    {
      "row": 1,
      "col": 0,
      "label": "B"
    },
    {
      "row": 1,
      "col": 1,
      "label": "C"
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
      "lineStyle": "dashed",
      "id": "a3",
      "label": "\\exists\\beta",
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
      "lineStyle": "solid",
      "id": "a2",
      "label": "\\gamma"
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
      "head": "epi",
      "lineStyle": "solid",
      "id": "a1",
      "label": "g",
      "labelPosition": "below"
    }
  ]
}
```
Diremos que ${}\mathcal{A}{}$ tiene suficientes proyectivos si ${}\forall A \in \mathcal{A}, \; \exists \alpha : P \twoheadrightarrow A$, donde ${}P{}$ es proyectivo. 
## Proposición
${}R\text{-Mod}$ tiene suficientes proyectivos
### Demostración
**TODO**