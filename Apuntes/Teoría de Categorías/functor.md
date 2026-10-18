# Functor
Sean ${}\mathcal{A}, \mathcal{B}{}$ [[Categoría|categorías]]. Un *functor* ${}F : \mathcal{A}\to \mathcal{B}{}$ consiste en:
- una función 
  $$
  \begin{align}
  \mathcal{A} &\to \mathcal{B} \\
  A & \mapsto FA
  \end{align}
  $$
- para cada ${}A, A' \in \mathcal{A}{}$, una función 
  $$
  \begin{align}
  \text{Hom}_{\mathcal{A}}(A, A') & \to \text{Hom}_{\mathcal{B}}(FA, FA') \\
  f  & \mapsto F(f)  
  \end{align}
  $$
cumpliendo los siguientes axiomas:
- ${}F(f' \circ f) = F(f')\circ F(f){}$, para todo ${}f \in \text{Hom}_{}(A, A'){}$ y ${}f' \in \text{Hom}_{}(A', A''){}$;
- ${}F(1_{A})=1_{F(A)}{}$,  para todo ${}A \in \mathcal{A}{}$.

# [[Functor]] exacto a derecha
Diremos que un functor ${}F:\mathcal{A}\to \mathcal{B}{}$ es *exacto a derecha* si para toda [[sucesión exacta]] corta ${}0 \to A \to B \to C\to 0{}$, la sucesión ${}FA\to FB\to FC \to 0{}$ es exacta.
## Proposición
Un functor ${}F:\mathcal{A}\to \mathcal{B}{}$ es exacto a derecha si y solo si mantiene la exactitud de sucesiones de la forma:
$$
P:\cdots \to  P_{2}\to P_{1}\to P_{0} \to 0
$$
### Demostración
**TODO**
