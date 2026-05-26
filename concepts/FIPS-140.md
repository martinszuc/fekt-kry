---
tags: [kry, concept, topic/standardy]
---
# FIPS 140 — Federal Information Processing Standard pre kryptografické moduly

**FIPS 140** (aktuálne verzia **FIPS 140-3**, od 2019) je americký vládny štandard definujúci bezpečnostné požiadavky na kryptografické moduly (HW aj SW).

**4 bezpečnostné úrovne:**
| Úroveň | Požiadavky |
|--------|-----------|
| **Level 1** | Základná kryptografia, žiadne fyzické požiadavky |
| **Level 2** | Dôkaz o neoprávnenom prístupe (tamper-evident) |
| **Level 3** | Ochrana pred prienikom (tamper-resistant), autentizácia obsluhy |
| **Level 4** | Kompletná fyzická ochrana, detekcia a zničenie kľúčov pri útoku |

**Relevancia:** Povinné pre kryptografické produkty predávané americkej vláde. Štandard v bankovníctve, zdravotníctve, obrane.

**Certifikácia:** CMVP (*Cryptographic Module Validation Program*) — NIST a CCCS.

---
## Spätné prepojenia
Kontext: [[Q13*]], [[Q43]]
Súvisí s: [[concepts/NIST-SP-800-90A]]
