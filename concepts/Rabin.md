---
tags: [kry, concept, topic/asymetria]
---
# Rabinov kryptosystém

**Rabinov kryptosystém** (Michael Rabin, 1979) je asymetrický systém, kde šifrovanie = umocnenie na druhú: $c = m^2 \bmod n$.

**Základ bezpečnosti:** Faktorizácia $n = pq$ — *matematicky dokázané* ako ekvivalentné dešifrovaniu.

**Kľúče:** Verejný $n = pq$; súkromný $(p, q)$.

**Problém:** Dešifrovanie vracia **4 kandidáty** na otvorený text (kvadratická nejednoznačnosť) → nutná redundancia v správe.

**Výhoda oproti RSA:** Prolomenie = faktorizácia (dôkaz existuje; u RSA chýba).

**Nevýhoda:** Zraniteľný na CCA (útočník dostane 4 odmocniny a vyfaktorizuje $n$).

---
## Spätné prepojenia
Detailne: [[Q31]]
Súvisí s: [[concepts/Faktorizacia]], [[concepts/CRT]], [[concepts/RSA]]
