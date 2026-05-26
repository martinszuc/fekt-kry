---
tags: [kry, concept, topic/kvantova]
---
# Groverov algoritmus

**Groverov algoritmus** (Lov Grover, 1996) je kvantový algoritmus na **prehľadávanie neštruktúrovanej databázy** v čase $O(\sqrt{N})$ namiesto klasického $O(N)$.

**Dopad na symetrickú kryptografiu:**
Efektívna bezpečnosť sa znižuje na **polovicu** (v bitoch):
| Algoritmus | Klasická bezpečnosť | Kvantová bezpečnosť (Grover) |
|------------|--------------------|-----------------------------|
| AES-128 | 128 bitov | **64 bitov** — nedostatočné |
| **AES-256** | 256 bitov | **128 bitov** — OK |
| SHA-256 kolízie | 128 bitov | 85 bitov — oslabené |
| **SHA-384** kolízie | 192 bitov | **128 bitov** — OK |

**Záver:** Symetrickú kryptografiu **nerozbije** — stačí zdvojnásobiť dĺžku kľúča (AES-128 → AES-256).

**Porovnanie so Shorom:** Grover = kvadratické zrýchlenie (zlé, ale not fatal). Shor = exponenciálne zrýchlenie (fatálne pre RSA/ECC).

---
## Spätné prepojenia
Kontext: [[Q14]], [[Q37]]
Súvisí s: [[concepts/Shorov-algoritmus]], [[concepts/AES]], [[concepts/SHA-2]]
