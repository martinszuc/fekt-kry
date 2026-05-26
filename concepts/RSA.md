---
tags: [kry, concept, topic/asymetria]
---
# RSA — Rivest–Shamir–Adleman

**RSA** je asymetrický kryptosystém navrhnutý Rivestom, Shamirom a Adlemanomv roku 1977. Je najpoužívanejším systémom s verejným kľúčom pre šifrovanie aj digitálne podpisy.

**Základ bezpečnosti:** Obtížnosť faktorizácie súčinu dvoch veľkých prvočísel $n = p \cdot q$.

**Kľúčové vzorce:**
- Generovanie: $n=pq$, $\varphi(n)=(p-1)(q-1)$, $ed \equiv 1 \pmod{\varphi(n)}$
- Šifrovanie: $c = m^e \bmod n$
- Dešifrovanie: $m = c^d \bmod n$
- Podpis: $s = H(m)^d \bmod n$; overenie: $H(m) = s^e \bmod n$

**Odporúčané dĺžky kľúčov:** 2048 bitov (minimum), 4096 bitov (dlhodobo).

**Slabiny raw RSA:** Pozri [[Q33]]. Opravy: [[concepts/OAEP]] (šifrovanie), [[concepts/PSS]] (podpisy).

**PQC hrozba:** Shorův algoritmus rieši faktorizáciu v polynomial. čase → [[Q37]], [[Q14]].

---
## Spätné prepojenia
Detailne: [[Q21]], [[Q22]], [[Q24]], [[Q33]], [[Q34]]
Súvisí s: [[concepts/Faktorizacia]], [[concepts/OAEP]], [[concepts/PSS]]
