***
# Formal Specification

## The Preservation Constraint

Let:
* $K$ = Total corpus of important knowledge regarding a domain (constituents + relations).
* $P$ = Explicitly stored information in the package (primitives + cached executable nodes).
* $L$ = Learner attributes (prior knowledge, working memory, inferential capacity).
* $t$ = Elapsed retention time interval.
* $u$ = Operational execution constraints (latency budgets, stress, context cues).
* $R(P, L, t)$ = Information learner $L$ can reliably reconstruct from $P$ at time $t$.

A representation qualifies as a viable concept package if and only if:

$$K \subseteq P \cup R(P, L, t)$$

---

## The Joint Cost Function

Subject to the preservation constraint, the optimal package $P^*$ minimizes storage footprint, reconstruction effort, and decay probability:

$$P^* = \arg\min_P \left[ C_{\text{storage}}(P) + C_{\text{compute}}(R(P, L, t)) + P_{\text{failure}}(P, L, t) \right]$$

Where:
* $C_{\text{storage}}$ measures cognitive footprint and memory footprint.
* $C_{\text{compute}}$ measures runtime latency and mental strain required to execute or derive un-cached nodes ($A \to \text{reasoning} \to B$).
* $P_{\text{failure}}$ measures the likelihood of derivation breakdown over retention horizon $t$.

---

## Learner Relativity

Optimal packages are learner-dependent functions:

$$P^* = f(K, L, t, u)$$

* **High-capacity learner ($L_{\text{expert}}$):** Retains $\{A, C, F\}$ and reconstructs $\{B, D, E, G, H\}$ on the fly.
* **Novice learner ($L_{\text{novice}}$):** Must store $\{A, B, C, D, F, H\}$ directly to guarantee recovery and fast execution across the same domain $K$.