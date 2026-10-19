# Poincaré MLR and Lorentz MLR

This repository provides implementations of multinomial logistic regression (MLR) in the **Poincaré** and **Lorentz** models of hyperbolic space.

When I started working with these formulations, one of the main challenges was understanding where the learnable parameters live and how the two formulations correspond. The key observation is that both methods use **Euclidean parameterizations of hyperbolic hyperplanes**, despite operating in different models of hyperbolic geometry.

This repository includes:

- the **Unidirectional Poincaré MLR** formulation from *Hyperbolic Neural Networks++ (HNN++)*; and
- the **Lorentz MLR** formulation from Bdeir et al.

The implementations are written using consistent notation and conventions to make their relationship explicit. In particular, the repository demonstrates numerically that, after matching the points, hyperplanes, parameter scales, and curvature conventions between the Poincaré and Lorentz models, the two formulations produce **identical logits up to numerical precision**.

The goal is to provide a compact reference for understanding and verifying the equivalence between these two hyperbolic MLR formulations.
