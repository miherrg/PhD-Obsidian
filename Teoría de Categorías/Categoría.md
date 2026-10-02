Una _categoría_ $\mathcal{A}$ consiste en:
- Una colección $\text{ob}(\mathcal{A})$ de _objetos_;
- $\forall A, B \in \text{ob}(\mathcal{A})$  una colección  ${}	\text{Hom}_{\mathcal{A}}(A, B){}$ de _morfismos_ entre ${}A{}$ y ${}B{}$;
- ${}\forall A, B, C \in \text{ob}(\mathcal{A}){}$,  una función 
  $$
  \begin{align}
  \text{Hom}_{}(A, B)  \times \text{Hom}_{}(B, C)  & \to   \text{Hom}_{}(A, C) \\
    (g,f) & \mapsto   g  \circ f
  \end{align}
  $$ llamada *composición*;
-  $\forall A \in \text{ob}(\mathcal{A})$, un elemento ${}1_{A}\in \text{Hom}(A,  A){}$ llamado *identidad* de A,
cumpliendo los siguientes axiomas:
- **Asociatividad:** $\forall f \in \text{Hom}_{}(A, B), \, g \in \text{Hom}_{}(B, C) \text{ y } h \in \text{Hom}_{}(C, D),$ tenemos que $(h \circ g) \circ f = h \circ (g \circ f)$;
- **Leyes de identidad:** $\forall f \in \text{Hom}_{}(A, B), \; \, f \circ 1_{A} = 1_{B}\circ f$.