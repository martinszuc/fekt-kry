---
tags: [kry, concept, topic/symetria]
---
# DES — Data Encryption Standard

**DES** je symetrická bloková šifra štandardizovaná NIST-om v roku 1977. Je dnes **zastaraná a nebezpečná** — 56-bitový kľúč je prelomiteľný brute-force.

**Parametre:** Blok 64 bitov, kľúč 56 bitov (+ 8 paritných = 64 bitov celkovo), 16 kôl Feistelova sieť.

**3DES (Triple DES):** Tri aplikácie DES ($E_{k1}(D_{k2}(E_{k1}(m)))$) — dnes tiež zastaraný.

**Náhrada:** [[concepts/AES]] (od 2001).

**Historický význam:** Prvý verejne štandardizovaný šifrovací algoritmus; formoval celú oblasť symetrickej kryptografie.

---
## Spätné prepojenia
Kontext: [[Q01]]
Náhrada: [[concepts/AES]]
