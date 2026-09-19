***
# Trade-offs, Compilation, and Redundancy

## 1. Minimal Storage vs. Runtime Execution (The JIT vs. AOT Trade-off)

Maximum compression (retaining only irreducible axiomatic primitives) produces high execution latency:

* **Pure Primitives (JIT Derivation):** Store only root axioms $A$. Every execution requires running $A \to \text{inference} \to B$. Zero redundancy, but prohibitive runtime latency.
* **Compiled Primitives (Cached Execution):** Retain $A + B$. Store the derived operational rule directly alongside its causal justification. Sacrifices minimal memory to achieve $O(1)$ or near-instant execution.

## 2. Redundancy as Error Correction Against Decay

Redundancy is decoupled from raw frequency of use:

$$\text{Needed Redundancy} \not\propto \text{Frequency of Use}$$
$$\text{Needed Redundancy} \propto \text{Risk of Reconstruction Failure}$$

| Usage Profile | Decay Risk | Optimal Packaging Strategy |
| :--- | :--- | :--- |
| **High-frequency execution** | Low (continuous active recall) | Strip redundant derivation paths; run lean bytecode |
| **Low-frequency execution** | High (interval forgetting) | High redundancy; preserve secondary causal anchors and reconstruction bridges |

Redundancy functions as error-correcting code across retention horizon $t$. If an inferential bridge decays, redundant cached anchors prevent complete failure of the mental model.