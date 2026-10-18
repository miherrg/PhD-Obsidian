# Tensor
Sea ${}R{}$ un anillo conmutativo y ${}M,N{}$ ${}R{}$-módulos. El *producto tensorial* ${}M\otimes_{R}N{}$ es un ${}R{}$-módulo junto a un morfismo bilineal ${}\otimes : M\times N \to M \otimes_{R}N{}$ tal que para todo morfismo bilineal ${}B :M\times N \to P{}$ existe un único homomorfismo ${}L : M \otimes_{R}N\to P{}$ que hace conmutar el siguiente diagrama:
```cd
{
  "version": 1,
  "rows": 3,
  "cols": 2,
  "cells": [
    {
      "row": 0,
      "col": 1,
      "label": "{M\\otimes_{R} N}"
    },
    {
      "row": 1,
      "col": 0,
      "label": "{M \\times N}"
    },
    {
      "row": 2,
      "col": 1,
      "label": "P"
    }
  ],
  "arrows": [
    {
      "id": "a3",
      "from": {
        "row": 0,
        "col": 1
      },
      "to": {
        "row": 2,
        "col": 1
      },
      "label": "\\exists!L",
      "head": "default",
      "lineStyle": "dashed"
    },
    {
      "id": "a1",
      "from": {
        "row": 1,
        "col": 0
      },
      "to": {
        "row": 0,
        "col": 1
      },
      "label": "\\otimes",
      "head": "default",
      "lineStyle": "solid"
    },
    {
      "id": "a2",
      "from": {
        "row": 1,
        "col": 0
      },
      "to": {
        "row": 2,
        "col": 1
      },
      "label": "B",
      "labelPosition": "below",
      "head": "default",
      "lineStyle": "solid"
    }
  ]
}
```
Por la universalidad de la definición, el producto tensorial es único.
## Nota
Si no da lugar a confusión, escribiremos ${}M\otimes N{}$ para denotar el producto tensorial.
## Teorema
${}M\otimes N{}$ existe.
### Demostración
**TODO**
## Proposición
Sean ${}M,N{}$ ${}R{}$-módulos. Entonces ${}\_\otimes N{}$ y ${}M \otimes \_{}{}$ son [[functor#Functor exacto a derecha|functores exactos a derecha]].
### Demostración
**TODO**