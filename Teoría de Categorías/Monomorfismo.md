Diremos que un morfismo, ${}i:A \to B{}$, es *mónico* (equivalentemente que ${}i{}$ es un monomorfismo) si ${}ig = 0 \implies g = 0{}$.  Para todo ${} {}g: A' \to A{} {}$

## Proposición
Todo [[núcleo]] es mónico.
### Demostración
Sea $f: A \to B{}$ un morfismo y sea $k: K \to A{}$ el núcleo de ${}f{}$.  Sea ${}g : K' \to {}K$ tal que ${}kg = 0{}$.
Tenemos que ${}f(kg) = f \circ 0 = 0{}$. Por la propiedad universal del núcleo, existe un único ${}u : K' \to K{}$ tal que ${} {}ku = kg = 0 = k \circ 0{} {}$. Por unicidad de ${}u{}$, ${}u = g = 0{}$, luego ${}k{}$ es mónico.