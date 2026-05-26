---
tags: [kry, concept, topic/autentizacia]
---
# Nonce — Number Used ONCE

**Nonce** (*Number used ONCE*) je náhodné alebo pseudonáhodné číslo generované raz pre jednu reláciu alebo jednu správu.

**Účel:** Dokazuje **čerstvosť** (*freshness*) správy — ak protistrana nonce zahrnie do odpovede, dokazuje, že správa vznikla v *tejto* relácii (nie replay z minulosti).

**Použitie:**
- **Autentizačné protokoly** — challenge-response (server pošle nonce, klient ho podpíše)
- **AES-GCM** — nonce/IV (12 bajtov) nesmie sa opakovať s rovnakým kľúčom!
- **TLS handshake** — `ClientHello.random` a `ServerHello.random` sú nonce
- **BAN logika** — $\#(N)$ = nonce $N$ je čerstvý ([[Q28]])

**Typy nonce:**
- Náhodný (random nonce) — kryptograficky bezpečný PRNG
- Sekvenčné číslo — rastúce počítadlo (jednoduchšie, ale sleduje históriu)
- Časová pečiatka — kombinácia s časovým oknom

---
## Spätné prepojenia
Kontext: [[Q26]], [[Q28]]
Súvisí s: [[concepts/BAN-logika]], [[concepts/Replay-attack]], [[concepts/AEAD]]
