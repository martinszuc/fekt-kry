---
tags: [kry, concept, topic/kodova, topic/pqc]
---
# Goppa kód

**Goppa kód** $\mathcal{G}(L, g)$ je trieda binárnych lineárnych opravných kódov definovaná polynómom $g(z)$ nad $\mathbb{GF}(2^m)$ a množinou $L$ prvkov telesa.

**Parametre:** $[n, k, d]$-kód:
- $n$ — dĺžka kódového slova
- $k$ — dimenzia (počet informačných bitov)
- $d = 2t+1$ — minimálna Hammingova vzdialenosť
- $t$ — maximálny počet opraviteľných chýb

**Kľúčová vlastnosť:** Existuje **efektívny dekódovací algoritmus** (Patterson, Berlekamp-Massey), ktorý opraví až $t$ chýb v $O(n^2)$ čase.

**Prečo v kryptografii:**
- Bez znalosti štruktúry ($S, G, P$ matíc) vyzerá Goppa kód ako náhodný kód.
- Dekódovanie *náhodného* kódu je NP-ťažký problém.
- McEliece ([[concepts/McEliece]]) a Niederreiter ([[concepts/Niederreiter]]) skrývajú Goppa kód za náhodnou maticou.

---
## Spätné prepojenia
Použitie: [[Q40]], [[Q41]]
Súvisí s: [[concepts/McEliece]], [[concepts/Niederreiter]]
