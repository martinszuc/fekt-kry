---
tags: [kry, concept, topic/symetria, topic/integrita]
---
# AEAD — Authenticated Encryption with Associated Data

**AEAD** (*Autentizované šifrovanie s pridruženými dátami*) je kryptografická primitíva, ktorá v jednom kroku poskytuje **dôvernosť + integritu + autentizáciu**.

**Vstup:** plaintext $m$, kľúč $k$, nonce $N$, asociované dáta $AD$ (šifrujú sa NEintimne, len overujú sa).
**Výstup:** šifrový text $c$ + autentizačný tag $t$.

**Hlavné AEAD schémy:**
| Algoritmus | Základ | Výkon |
|-----------|--------|------|
| **AES-GCM** | AES-CTR + GHASH | Veľmi rýchly s HW (AES-NI) |
| **AES-CCM** | AES-CTR + CBC-MAC | IoT, vhodné pre obmedzené CPU |
| **ChaCha20-Poly1305** | ChaCha20 + Poly1305 | Rýchly SW, bez nutnosti HW |
| **ASCON-128** | Sponge permutácia | Navrhnutý pre IoT (NIST LWC 2023) |

**Kľúčová vlastnosť:** Nonce sa nesmie nikdy opakovať s rovnakým kľúčom (tzv. „nonce-misuse" = katastrofálna bezpečnosť pre GCM).

---
## Spätné prepojenia
Použitie: [[Q04]], [[Q43]]
Súvisí s: [[concepts/AES]], [[concepts/ChaCha20]], [[concepts/MAC]]
