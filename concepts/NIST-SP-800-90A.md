---
tags: [kry, concept, topic/standardy, topic/rng]
---
# NIST SP 800-90A — Odporúčanie pre kryptograficky bezpečné RNG

**NIST SP 800-90A** je dokument odporúčajúci implementácie **DRBG** (*Deterministic Random Bit Generator*) — kryptograficky bezpečných pseudonáhodných generátorov.

**Tri schválené DRBG:**
| Meno | Základ | Poznámka |
|------|--------|---------|
| **Hash_DRBG** | SHA-256/384/512 | Jednoduchý, pomalý |
| **HMAC_DRBG** | HMAC-SHA-256/384 | Odporúčaný pre väčšinu aplikácií |
| **CTR_DRBG** | AES-CTR | Rýchly, s HW AES |

**Kontroverzný Dual_EC_DRBG** (eliptické krivky) bol stiahnutý — odborníci objavili pravdepodobné NSA backdoor (2013, Snowden dokumenty).

**Použitie:** Generovanie kryptografických kľúčov, nonce hodnôt, inicializačných vektorov.

---
## Spätné prepojenia
Detailne: [[Q13*]], [[Q43]]
Súvisí s: [[concepts/FIPS-140]]
