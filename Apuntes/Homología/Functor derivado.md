# [[Functor]] derivado a izquierda
Sea ${}F : \mathcal{A}\to \mathcal{B}{}$ un [[functor]] exacto a derecha, con ${}\mathcal{A}{}$ una [[categoría abeliana]] con suficientes [[proyectivos]]. ${}\forall i \ge 0{}$ definimos el *${}i{}$-ésimo functor derivado a izquierda de ${}F{}$* de la siguiente forma: dado ${}A\in \mathcal{A}{}$ y ${}P\overset{\epsilon}{\to}A{}$ una [[resolución]] proyectiva:
$$
L_{i}F(A) :=H_{i}(F(P))
$$
Notemos que, al ser ${}F{}$ exacto a derecha, ${}FP_{1}\to FP_{0}\to FA \to 0{}$ es exacta. Por tanto ${}{L_{0}\, F(A)} = H_{0}(F(P)) \cong FA{}$.
**TODO: Demostrar esto de forma categórica y no con módulos.**
## Lema
Los objetos ${}L_{i}F(A){}$ están bien definidos bajo isomorfismo. Es decir, si ${}Q \overset{\eta}{\to} A{}$ es otra resolución proyectiva de ${}A{}$, entonces existe un isomorfismo canónico
$$
H_{i}(F(P)) \cong H_{i}(F(Q))
$$
### Demostración
**TODO**