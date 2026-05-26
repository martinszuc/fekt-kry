---
tags: [kry, concept, topic/asymetria, topic/podpisy]
---
# PSS — Probabilistic Signature Scheme

**RSA-PSS** (*Probabilistic Signature Scheme*) je kryptografické doplnenie pred RSA podpisovaním. Štandard: PKCS#1 v2.x, RFC 8017.

**Účel:** Nahradiť deterministický PKCS#1 v1.5 podpis — pridáva soľ (*salt*) pre náhodnosť a poskytuje dokazateľnú bezpečnosť.

**Princíp:**
1. Haš správy + náhodná **soľ** → kombinovaný vstup $M'$
2. Haš $M'$ → $H$; soľ + padding → $DB$; $DB$ XOR MGF(H) = $maskedDB$
3. Zakódovaná správa $EM$ prechádza RSA podpisovaním

**Bezpečnostný model:** EUF-CMA (v modeli náhodného orákula) — prolomenie PSS = invertovanie RSA.

**Dôležité:** PSS je len pre **podpisy** — pre šifrovanie sa používa [[concepts/OAEP]].

---
## Spätné prepojenia
Detailne: [[Q34]], Slabiny raw RSA: [[Q33]]
Súvisí s: [[concepts/OAEP]], [[concepts/RSA]]
