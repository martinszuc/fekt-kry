---
tags: [kry, concept, topic/symetria]
---
# ChaCha20 — prúdová šifra

**ChaCha20** je symetrická prúdová šifra navrhnutá Danielom J. Bernsteinom (2008). Je modernálternatívou k AES pre platformy bez hardvérovej AES akcelerácie.

**Parametre:** 256-bitový kľúč, 96-bitový nonce, 32-bitový counter → generuje kľúčový prúd.

**Princíp:** 20 kôl operácií Add-Rotate-XOR (ARX) na 4×4 matici 32-bitových slov — jednoduchá, rýchla softvérová implementácia.

**Kombinovaná forma — ChaCha20-Poly1305:**
- ChaCha20 šifruje dáta (prúdová šifra)
- Poly1305 overuje integritu (MAC)
- Spolu tvoria **AEAD** schému (RFC 8439)

**Výhody oproti AES-GCM:**
- Rýchlejší bez HW akcelerácie (ARM, MIPS)
- Odolný voči timing útokům (ARX = konštantný čas)
- Nonce-misuse odolnejší (XSalsa20 variant)

**Použitie:** TLS 1.3, WireGuard, SSH, Signal protokol.

---
## Spätné prepojenia
Kontext: [[Q01]], [[Q04]]
Súvisí s: [[concepts/AEAD]], [[concepts/AES]]
