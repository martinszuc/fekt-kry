---
tags: [kry, concept, topic/pqc, topic/mriazka]
---
# Dilithium / ML-DSA — postkvantový digitálny podpis

**ML-DSA** (pôvodne *Dilithium*) je postkvantový algoritmus digitálneho podpisu štandardizovaný NIST-om v roku 2024 ako **FIPS 204**.

**Základ:** Module-LWE/Module-SIS nad polynomiálnym okruhom.

**Varianty:**
| Variant | Bezpečnosť | Verejný kľúč | Podpis |
|---------|-----------|-------------|-------|
| ML-DSA-44 | 128-bit | 1312 B | 2420 B |
| ML-DSA-65 | 192-bit | 1952 B | 3293 B |
| ML-DSA-87 | 256-bit | 2592 B | 4595 B |

**Použitie:** Náhrada ECDSA/RSA v post-kvantovom prostredí; TLS certifikáty, kódové podpisy.

---
## Spätné prepojenia
Kontext: [[Q37]], [[Q39]]
Súvisí s: [[concepts/LWE]], [[concepts/Kyber]]
