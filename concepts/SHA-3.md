---
tags: [kry, concept, topic/has]
---
# SHA-3 — Secure Hash Algorithm 3 (Keccak)

**SHA-3** je rodina hašovacích funkcií štandardizovaná NIST-om v roku 2015 (FIPS 202). Interný algoritmus: **Keccak** (autori: Bertoni, Daemen, Peeters, Van Assche).

**Kľúčový rozdiel od SHA-2:** SHA-3 používa **hubovú konštrukciu (Sponge construction)**, nie Merkle-Damgård. Preto nie je náchylná na *length extension attack*.

**Varianty:**
| Variant | Výstup | Bezpečnosť |
|---------|--------|-----------|
| SHA3-224 | 224 bitov | 112-bit |
| SHA3-256 | 256 bitov | 128-bit |
| SHA3-384 | 384 bitov | 192-bit |
| SHA3-512 | 512 bitov | 256-bit |
| **SHAKE128** | ľubovoľný (XOF) | 128-bit |
| **SHAKE256** | ľubovoľný (XOF) | 256-bit |

**XOF** (*Extendable-Output Function*) — funkcia s premenlivou dĺžkou výstupu; SHAKE128/256 sú XOF funkcie.

**Použitie:** Digitálne podpisy, MAC, derivácia kľúčov, post-kvantová kryptografia (SPHINCS+).

---
## Spätné prepojenia
Princíp konštrukcie: [[Q08]]
Súvisí s: [[concepts/SHA-2]], [[concepts/Sponge-construction]], [[concepts/Merkle-Damgard]]
