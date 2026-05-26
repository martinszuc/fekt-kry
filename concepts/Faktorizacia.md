---
tags: [kry, concept, topic/matematika]
---
# Faktorizácia — Integer Factorization Problem

**Problém faktorizácie** spočíva v nájdení prvočíselného rozkladu $n = p \cdot q$ pre dané $n$.

**Jednosmerná funkcia:** Násobenie je rýchle ($O(\log^2 n)$), faktorizácia je ťažká — neexistuje polynomiálny klasický algoritmus.

**Kryptosystémy závislé na faktorizácii:**
- **RSA** — [[concepts/RSA]] — šifrovanie a podpisy
- **Rabinov systém** — [[concepts/Rabin]] — prolomenie = faktorizácia (dokázané)

**Najlepšie klasické algoritmy:**
- General Number Field Sieve (GNFS): $O(e^{1.9 (\log n)^{1/3} (\log \log n)^{2/3}})$
- Pre 2048-bit RSA: $\approx 10^{25}$ operácií

**PQC hrozba:** Shorův algoritmus faktorizuje polynomiálne → RSA je kvantovo-zraniteľné.

---
## Spätné prepojenia
Detailne: [[Q24]], [[Q31]]
Súvisí s: [[concepts/RSA]], [[concepts/Rabin]], [[concepts/Shorov-algoritmus]]
