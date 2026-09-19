***
# Information Preservation Value

Information has no inherent preservation value. Its value is relative to an **agent**, that agent's possible future objectives, and the structure of the agent's existing knowledge.

The central problem is not simply "Is this information useful now?" but:

> **Does preserving this information protect meaningful future capability?**

## 1. Objective-Relative Relevance

You cannot evaluate information without an objective. The objective determines what information is relevant.

When the future objective is unknown, the meta-objective becomes **preserving optionality**: retain information that keeps valuable future paths open.

This connects to [[abstraction & relevance]] and [[selective forgetting]].

## 2. Case Utility

General applicability matters because broadly useful information applies across more possible future cases. However, generality is not fundamental.

A narrow piece of information may be more valuable than a general principle if the cases in which it matters are sufficiently important.

Therefore, preservation value should be evaluated across possible future cases:

$$
V_{direct}(i)=\sum_{c \in C} P(c)\cdot U(i,c)
$$

where:
- $P(c)$ = likelihood or relevance of future case $c$
- $U(i,c)$ = utility provided by information $i$ in that case

**Generality increases the number of useful cases; significance increases the value within those cases.**

## 3. Structural Value

Information should not be evaluated only in isolation. Knowledge exists as structures and relationships.

A piece of information can have low standalone utility while being extremely valuable because it acts as:
- a bridge between concepts;
- a prerequisite;
- a reconstruction path;
- a compression key;
- an index into other knowledge.

Its usefulness may therefore be its structural role itself.

$$
V(i)=V_{direct}(i)+V_{structural}(i)
$$

This connects to [[knowledge graph hypothesis]] and [[knowledge prerequisite hierarchy]].

## 4. Reconstructibility

Two equally useful pieces of information should not necessarily be preserved equally.

If one can be cheaply and reliably reconstructed later, losing it has little permanent cost. If another is difficult or impossible to reconstruct, deletion destroys future optionality.

Reconstructibility therefore modifies preservation value:

- **Easy to reconstruct** → lower need for preservation.
- **Hard or impossible to reconstruct** → higher need for preservation, assuming meaningful case utility exists.

This is consistent with [[tradeoffs & redundancy]].

## 5. Safe Forgetting

The strongest deletion criterion is:

> **Information can be safely forgotten when it has no meaningful direct value, no meaningful structural value, and no irreplaceable reconstruction role for the agent.**

Because future objectives are uncertain, absolute zero is usually impossible to prove. The practical rule is therefore:

$$
\text{Forget } i \text{ when expected preservation value} \leq \text{retention + maintenance cost}
$$

Preservation is justified only when keeping the information protects more future capability than it costs to retain.

## Core Principle

> **Preserve information according to the future capability it protects, not according to how interesting, detailed, general, or currently useful it appears.**

Generality, significance, structural position, and reconstructibility are all components of that deeper quantity: **preservation value**.
***
