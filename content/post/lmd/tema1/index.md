---
title: tema1
date: 2024-02-26
tags: [lmd]
---

# Algebra de Boole

Sea \\(B\\) un coonjunto, se dice que \\(B\\) tiene estructura de álgebra de Boole si está dotado de dos operaciones binarias, \\(\vee\\) y \\(\wedge\\) que satisfacen las siguientes propiedades:

$$
\begin{aligned}
\text{Asociativa: } & \forall x, y, z \in B \quad (x \vee y) \vee z = x \vee (y \vee z) \\
\text{Conmutativa: } & \forall x, y, z \in B \quad x \vee y = y \vee x \\
\text{Distributiva: } & \forall x, y, z \in B \quad x \wedge (y \vee z) = (x \wedge y) \vee (x \wedge z) \\
\text{Elementos neutros: } & \forall x \in B \quad \exists 0,1 \in B \text{ tal que } x \vee 0 = x \text{ y } x \wedge 1 = x \\
\text{Existencia de complementos: } & \forall x \in B \quad \exists x' \in B \text{ tal que } x \vee x' = 1 \text{ y } x \wedge x' = 0 \\
\end{aligned}
$$

*Ejemplo:* Sea \\(X\\) un conjunto. El conjunto \\(P(X)\\), donde \\(P(X)\\) es el conjunto de todos los subconjuntos de \\(X\\), con las operaciones de unión y de intersección, tiene estructura de álgebra de Boole.

$$
P(x) = \{ A \mid A \subseteq X \}
$$

por ejemplo, si \\(X = \{a, b, c\}\\), 

$$
P(X) = \{ \{\varnothing\} , \{a\}, \{b\}, \{c\}, \{a, b\}, \{a, c\}, \{b, c\}, \{a, b, c\} \} 
\#(P(X)) = 2^{\#(X)} = 2^3 = 8
$$

En general, si \\(X\\) es un conjunto finito, entonces \\(\#(P(X)) = 2^{\#(X)}\\)

## Ejemplos de estructuras de álgebra de Boole


1. **Conjunto Boleano Clásico \\(B = \{0, 1\}\\):**

   - **Operaciones:**
     - \\(\vee\\) (Disyunción): \\(0 \vee 0 = 0, \quad 0 \vee 1 = 1, \quad 1 \vee 0 = 1, \quad 1 \vee 1 = 1\\)
     - \\(\wedge\\) (Conjunción):\\(0 \wedge 0 = 0, \quad 0 \wedge 1 = 0, \quad 1 \wedge 0 = 0, \quad 1 \wedge 1 = 1\\)

   - **Propiedades:**
     - Asociativa: \\((x \vee y) \vee z = x \vee (y \vee z)\\) y \\((x \wedge y) \wedge z = x \wedge (y \wedge z)\\)
     - Conmutativa: \\(x \vee y = y \vee x\\) y \\(x \wedge y = y \wedge x\\)
     - Distributiva: \\(x \wedge (y \vee z) = (x \wedge y) \vee (x \wedge z)\\)

   - **Elementos neutros y complementos:**
     - \\(0\\) es el elemento neutro para \\(\vee\\) y \\(1\\) es el elemento neutro para \\(\wedge\\).
     - Cada elemento \\(x\\) tiene su complemento \\(x'\\) tal que \\(x \vee x' = 1\\) y \\(x \wedge x' = 0\\).
