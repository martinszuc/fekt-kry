---
tags: [kry, concept, topic/pqc, topic/mriazka]
---
# LWE — Learning With Errors

**LWE** (*Learning With Errors*) je kryptografický ťažký problém navrhnutý Odedom Regevom (2005). Je základom mriežkovej postkvantovej kryptografie.

**Vzťah:** $\mathbf{b} = A\mathbf{s} + \mathbf{e} \pmod{q}$

- $A$ — verejná náhodná matica (koeficienty rovníc)
- $\mathbf{s}$ — tajný vektor (súkromný kľúč)
- $\mathbf{e}$ — malý Gaussov šum (kľúč k bezpečnosti)
- $\mathbf{b}$ — verejný vektor

**Prečo ťažké:** Šum $\mathbf{e}$ znemožňuje Gaussovu elimináciu → ekvivalentné SVP (Shortest Vector Problem) v mriežke — NP-ťažký problém.

**Varianty:**
- **Ring-LWE (R-LWE)** — polynómy namiesto matíc
- **Module-LWE (M-LWE)** — matice polynómov → základ Kyber, Dilithium

---
## Spätné prepojenia
Princíp: [[Q38]], Porovnanie: [[Q39]]
Súvisí s: [[concepts/Kyber]], [[concepts/Dilithium]], [[concepts/Mriežková-kryptografia]]
