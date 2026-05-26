---
tags: [kry, concept, topic/protokoly]
---
# TLS — Transport Layer Security

**TLS** (*Transport Layer Security*) je kryptografický protokol zabezpečujúci dôvernosť, integritu a autentizáciu pri prenose dát cez sieť. Nástupca SSL.

**Aktuálna verzia: TLS 1.3** (RFC 8446, 2018).

**Hlavné fázy (TLS 1.3):**
1. **Handshake** — výmena kľúčov (ECDHE), autentizácia servera (certifikát + EdDSA/ECDSA)
2. **Record Protocol** — šifrovanie dát (AES-256-GCM alebo ChaCha20-Poly1305)

**TLS 1.3 vs. 1.2:**
- Odstránené slabé šifrovacie sady (RC4, 3DES, RSA key exchange)
- Povinný PFS (ECDHE)
- 1-RTT handshake (rýchlejší)
- 0-RTT pre opakované spojenia (s obmedzenou ochranou replay)

**Použitie:** HTTPS, IMAPS, SMTPS, FTPS, VoIP (DTLS pre UDP).

---
## Spätné prepojenia
Kontext: [[Q43]]
Súvisí s: [[concepts/PKI]], [[concepts/AEAD]], [[concepts/PFS]]
