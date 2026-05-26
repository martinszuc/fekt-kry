---
tags: [kry, concept, topic/integrita]
---
# MAC — Message Authentication Code

**MAC** (*Kód autentizácie správy*) je krátka hodnota vypočítaná zo správy a **tajného kľúča** — zaručuje **integritu a autentičnosť** správy, ale *nie* nepopierateľnosť (obaja majú kľúč).

**Typy MAC:**
- **HMAC** — hašovacia funkcia + kľúč ([[concepts/HMAC]])
- **CMAC / OMAC** — bloková šifra (AES-CMAC)
- **Poly1305** — polynomiálna MAC (používaná s ChaCha20)
- **GHASH** — v AES-GCM (AEAD)

**Rozdiel od digitálneho podpisu:** MAC vyžaduje zdieľaný tajný kľúč (symetrická auth.); podpis používa asymetrický pár kľúčov a poskytuje nepopierateľnosť.

**Použitie:** TLS record layer, IPsec, SRTP, API tokeny.

---
## Spätné prepojenia
Kontext: [[Q03]], [[Q04]]
Súvisí s: [[concepts/HMAC]], [[concepts/AEAD]]
