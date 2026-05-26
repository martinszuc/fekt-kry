---
tags: [kry, concept, topic/pqc, topic/mriazka]
---
# Mriežková kryptografia (Lattice-based Cryptography)

**Mriežková kryptografia** je najväčšia rodina postkvantovej kryptografie. Bezpečnosť stojí na obtížnosti mriežkových problémov.

**Čo je mriežka (lattice):** Diskrétna periodická štruktúra v $n$-rozmernom priestore; formálne $\mathcal{L} = \{Av : v \in \mathbb{Z}^n\}$ pre bázu $A$.

**Kľúčové problémy:**
- **SVP** (*Shortest Vector Problem*) — nájdi najkratší nenulový vektor mriežky
- **LWE** (*Learning With Errors*) — [[concepts/LWE]]

**Prečo kvantovo-bezpečné:** Groverov ani Shorův algoritmus neponúkajú exponenciálne zrýchlenie pre SVP/LWE.

**Štandardy (NIST 2024):**
- [[concepts/Kyber]] / ML-KEM (FIPS 203) — výmena kľúčov
- [[concepts/Dilithium]] / ML-DSA (FIPS 204) — podpisy

---
## Spätné prepojenia
Detailne: [[Q37]], [[Q38]], [[Q39]]
Súvisí s: [[concepts/LWE]], [[concepts/Kyber]], [[concepts/Dilithium]]
