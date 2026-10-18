# Resolución proyectiva
Sea ${}A \in \mathcal{A}{}$, una resolución proyectiva de ${}A{}$ es un [[Complejo de cadenas]] ${}P \in \text{Ch}(\mathcal{A}){}$, donde todos los ${}P_{n}{}$ son [[Proyectivos]] y ${}P_{n} = 0,\; \forall n < 0{}$, junto a un morfismo ${}p : P_{0} \to A{}$ de tal forma que la siguiente sucesión es [[sucesión exacta|exacta]].
```cd
{
  "version": 1,
  "rows": 2,
  "cols": 5,
  "cells": [
    {
      "row": 1,
      "col": 0,
      "label": "\\cdots"
    },
    {
      "row": 1,
      "col": 1,
      "label": "P_1"
    },
    {
      "row": 1,
      "col": 2,
      "label": "P_0"
    },
    {
      "row": 1,
      "col": 3,
      "label": "A"
    },
    {
      "row": 1,
      "col": 4,
      "label": "0"
    }
  ],
  "arrows": [
    {
      "id": "a19",
      "from": {
        "row": 1,
        "col": 0
      },
      "to": {
        "row": 1,
        "col": 1
      },
      "label": "d_2",
      "head": "default",
      "lineStyle": "solid"
    },
    {
      "id": "a20",
      "from": {
        "row": 1,
        "col": 1
      },
      "to": {
        "row": 1,
        "col": 2
      },
      "label": "d_1",
      "head": "default",
      "lineStyle": "solid"
    },
    {
      "id": "a21",
      "from": {
        "row": 1,
        "col": 2
      },
      "to": {
        "row": 1,
        "col": 3
      },
      "label": "p",
      "head": "default",
      "lineStyle": "solid"
    },
    {
      "id": "a22",
      "from": {
        "row": 1,
        "col": 3
      },
      "to": {
        "row": 1,
        "col": 4
      },
      "head": "default",
      "lineStyle": "solid"
    }
  ]
}
```
Para abreviar, denotaremos las resoluciones proyectivas como ${}P \overset{p}{\to}A{}$, donde ${}A{}$ es el objeto, ${}P{}$ el [[complejo de cadenas]] y ${}p:P_{0} \to A{}$  o como ${}\mathcal{P}{}$.
## Lema
Sea ${}\mathcal{A}{}$ una [[Categoría abeliana]] con suficientes [[Proyectivos]]. Entonces ${}\forall M \in \mathcal{A}{}$ tiene una resolución proyectiva.
### Demostración
**TODO**
## Teorema
Sea ${}P \overset{\epsilon}{\to} M{}$ una resolución proyectiva de ${}M{}$ y ${}f' : M \to N{}$ un morfismo en ${}\mathcal{A}{}$. Entonces, para toda resolución proyectiva ${}Q\overset{\eta}{\to}N{}$,  hay un [[morfismo de cadenas]] ${}f:P \to Q{}$ levantando ${}f'{}$, es decir, ${}\eta f_{0} = f'\epsilon{}$. El morfismo ${}f{}$ es único salvo [[Homotopía de cadenas|equivalencia homotópica de cadenas]].
### Demostración
**TODO**