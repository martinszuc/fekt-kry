---
tags: [kry, concept, topic/asymetria]
---
# OAEP — Optimal Asymmetric Encryption Padding

**OAEP** (*Optimal Asymmetric Encryption Padding*) je kryptografické doplnenie správy pred RSA šifrovaním. Štandard: PKCS#1 v2.x, RFC 8017.

**Účel:** Opraviť slabiny *raw RSA* — determinizmus, malé hodnoty, CCA2 zraniteľnosť.

**Princíp (Feistelová štruktúra):**
1. Pridáva **náhodný seed** → randomizácia (každý šifrový text iný)
2. Správa + seed sa navzájom „pomiešajú" pomocou MGF (Mask Generation Function)
3. Výsledok prechádzajú RSA exponenciáciou

**Bezpečnostný model:** IND-CCA2 (v modeli náhodného orákula) — odolnosť voči adaptívnemu útoku zvoleným šifrovým textom.

**Dôležité:** OAEP je len pre **šifrovanie** — pre podpisy sa používa [[concepts/PSS]].

---
## Spätné prepojenia
Detailne: [[Q34]], Slabiny raw RSA: [[Q33]]
Súvisí s: [[concepts/PSS]], [[concepts/RSA]]
