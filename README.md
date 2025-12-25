# Quantum Simulation of Black Hole Evaporation

## Overview
This repository is a conceptual and computational study of black hole evaporation using simplified qubit models, with a focus on understanding:
- Why hawking's semiclassical picture leads to information loss
- Why small corrections cannot restore unitarity(Mathur's bound)
- How different toy models fail or succeed in reproducing Page Curve.
- How the Avery qubit model evades Mathur's no-go theorem.

## Motivation 
The Black Hole information paradox arises from a tension between:
- Local quantum field theory at the horizon.
- Unitarity of quantum mechanics

  While Hawking's original calculation predicts monotonic growth of entanglement entropy, Page's argument suggest a unitary evaporation process must exhibit a Page curve.

  This repository explores why most intuitive fixes fail and what structural changes are required for information recovery.

## Conceptual Framework: Page, Mathur and Avery
### The Information-Theoretic Benchmark (Page)
The entanglement entropy of radiation emitted from a finite quantum system undergoing unitary evolution is constrained by general principles of quantum information theory. Page curve argument
showed that, for a pure initial state, the radiation entropy must initially increase, reach a maximum at the Page time, then decrease to zero as evaporation completes.

This result is independent of gravity and provides a model-agnostic benchmark for black hole evaporation. Any unitary evaporation model must reproduce this Page curve behaviour.

### The No-Go Constraint(Mathur)
While Page's argument specifies what must happen, it does not explain how information escapes from a black hole. Mathur small correction theorem addressed this question by analyzing whether small corrections
to Hawking's semiclassical pair creation process could restore unitarity.

Using strong subadditivity of entanglement entropy, Mathur demonstrated that if deviations from Hawking radiation are perturbatively small at each emission step, then the entanglement entropy of the radiation must continue to grow monotonically.
This result, often referred to as Mathur's bound, establishes that small corrections cannot accumulate to produce Page curve.

Thus mathur's argument imposes a sharp constraint:
Any unitary model of black hole evaporation must involve order-unity modifications to the semiclassical picture.

### The allowed solution space(Avery)
Given the combined constraints of Page and Mathur, a viable model must:
- be globally unitary,
- allow non-purturbative information transfer,
- and explicitly violate at least one assumption underlying Mathur's bound.

Avery qubit evaporation model provides a controlled qubit-based framework to explore such models. Rather than proposing a specific microscopic theory of quantum gravity, the 
Avery model contructs explicit unitary evaporation maps and tracks entanglement entropy step by step.

This framwork allows:
- direct testing of Mathur's stability argument,
- explicit idnetification of which assumptions are violated,
- and controlled reproduction of the Page curve.

In this project, the Avery model serves as the constructive endpoint of the analysis: after demonstrating why locality-preserving and small-correction model fails,
we use the Avery framework to show how unitary evaporation consistent with the Page curve can occur.


**In summary**
Page tells us what the entropy must do, Mathur tells us what cannot make it happen, & Avery provides a controlled framework to explore what can.
## Section-by-Section Description
  1. Mathur's Stability Test(No Black Hole model)
 
     We begin with pure quantum information toy models, independent of gravity, to demonstrate:
     - Why entanglement is not additive.
     - Why small corrections do not lead to small entanglement changes.
     - Why entropy growth is stable under perturbations.
    
       This isolates the paradox as a quantum-information problem, not a geometric one.
    
  2. Black Hole-Inspired Toy Models
 
     We then introduce models motivated by black hole evaporation:
     - Hawking model (pair creation, local, non-unitary)
     - Burning paper analogy(unitary benchmark)
     - Impure and non-invertible models
     - Mathur's shift/anti-shift model
     - Mathur's Ising spin model
    
       Each model is analyzed with:
       - Explicit assumptions
       - Step-by-step evaporation
       - ENtanglement entropy tracking
       - Clear explanation of why it fails or succeeds
      
  3. Page Curve simulations
 
       For each model, we compute:
       - Radiation entropy as a function of evaporation step
       - Comparison with expected page behaviour
      
  4. Transition to the Avery Qubit Model
 
       After exhausting all locality-preserving and small-correction models, we motivate the need for:
       - Order unity information transfer
       - Explicit unitary evolution
       - Strong coupling between black hole and radiation degree of freedom
      
         This leads naturally to the Avery qubit model, which is studied in detail.

  5. Avery Qubit Model
 
       We implement:
       - Avery's unitary evaporation maps
       - Step-by-Step qubit evolution
       - Explicit tracking of information flow
       - Successful reproduction of the Page curve
      
       We also explain which assumption of Mathur's bound is violated and why this does not contradict unitarity.


  ## Key results
  - Small corrections to Hawking radiation cannot restore unitarity.
  - Entanglement entropy growth is non-perturbatively stable.
  - Page curve recovery requires order-unity correlations per emission.

## References

[1] Avery, Steven G. “Qubit Models of Black Hole Evaporation.” Journal of High Energy Physics 2013, no. 1 (2013): 176. https://doi.org/10.1007/JHEP01(2013)176.

[2] Rahman, Imran Abdul, and Toby Wiseman. On the Black Hole Information Paradox and the Page Curve. n.d.


 
       

       
  

