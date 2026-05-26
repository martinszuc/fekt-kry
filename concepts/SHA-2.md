---
tags: [kry, concept, topic/has]
---
# SHA-2 — Secure Hash Algorithm 2

**SHA-2** je rodina hašovacích funkcií navrhnutá NSA, štandardizovaná NIST-om (FIPS 180-4). Používa **Merkle-Damgård konštrukciu**.

**Varianty:**
| Variant | Výstup | Bezpečnosť |
|---------|--------|-----------|
| SHA-224 | 224 bitov | 112-bit |
| SHA-256 | 256 bitov | 128-bit |
| SHA-384 | 384 bitov | 192-bit |
| SHA-512 | 512 bitov | 256-bit |

**Slabina:** Náchylná na *length extension attack* (dedená z Merkle-Damgård) — preto sa používa **HMAC-SHA256** namiesto holého SHA-256 pre MAC. Pozri [[Q07]].

**Kvantová odolnosť:** SHA-256 s Groverom = 85-bit bezpečnosť. SHA-384 = 192-bit → bezpečné. Pozri [[Q14]].

**Použitie:** TLS certifikáty, Bitcoin, kódové podpisy, HMAC.

---
## Spätné prepojenia
Konštrukcia: [[Q07]], [[concepts/Merkle-Damgard]]
Porovnanie: [[concepts/SHA-3]]
