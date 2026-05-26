---
tags: [kry, concept, topic/pqc, topic/mriazka]
---
# Kyber / ML-KEM — postkvantová výmena kľúčov

**ML-KEM** (pôvodne *Kyber*) je postkvantový KEM (*Key Encapsulation Mechanism*) štandardizovaný NIST-om v roku 2024 ako **FIPS 203**.

**Základ:** Module-LWE nad polynomiálnym okruhom $\mathbb{Z}_q[x]/(x^{256}+1)$.

**Varianty (bezpečnostné úrovne):**
| Variant | $k$ | Bezpečnosť | Verejný kľúč |
|---------|-----|-----------|-------------|
| ML-KEM-512 | 2 | 128-bit | 800 B |
| ML-KEM-768 | 3 | 192-bit | 1184 B |
| ML-KEM-1024 | 4 | 256-bit | 1568 B |

**Porovnanie:** RSA-2048 verejný kľúč = 256 B, ale Kyber je 1000× rýchlejší pri výmene kľúčov.

**Použitie:** TLS 1.3 hybridná výmena kľúčov (X25519+Kyber768), Signal protokol (2023+).

---
## Spätné prepojenia
Kontext: [[Q37]], [[Q38]], [[Q39]]
Súvisí s: [[concepts/LWE]], [[concepts/Dilithium]]
