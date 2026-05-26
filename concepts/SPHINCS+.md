---
tags: [kry, concept, topic/pqc, topic/hasova]
---
# SPHINCS+ / SLH-DSA — hašový postkvantový podpis

**SLH-DSA** (pôvodne *SPHINCS+*) je postkvantový algoritmus digitálneho podpisu štandardizovaný NIST-om v roku 2024 ako **FIPS 205**.

**Základ:** Bezpečnosť závisí **výlučne od bezpečnosti hašovacej funkcie** (SHA-256 alebo SHAKE256) — najkonzervatívnejšie predpoklady.

**Stavba:** Strom Merkle zložený z WOTS+ (Winternitz OTS — [[Q10]]) jednorazových podpisov.

**Parametre:** Veľké podpisy (8–50 KB) — nevýhoda oproti Dilithium, ale maximálna konzervativita.

**Varianty:** SPHINCS+-SHAKE-128s, SPHINCS+-SHA2-256s, atď.

---
## Spätné prepojenia
Kontext: [[Q37]], [[Q09]], [[Q10]]
Súvisí s: [[concepts/SHA-3]], [[concepts/Dilithium]]
