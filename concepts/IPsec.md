---
tags: [kry, concept, topic/protokoly]
---
# IPsec — Internet Protocol Security

**IPsec** je sústava protokolov pre zabezpečenie IP komunikácie na sieťovej vrstve (L3). Štandard: RFC 4301+.

**Dva módy:**
- **Transportný mód** — šifruje len payload; IP hlavička viditeľná
- **Tunelovací mód** — šifruje celý pôvodný paket (vrátane IP hlavičky) → Site-to-Site VPN

**Kľúčové protokoly:**
- **AH** (*Authentication Header*) — len integrita a autentizácia (bez šifrovania)
- **ESP** (*Encapsulating Security Payload*) — dôvernosť + integrita + autentizácia
- **IKEv2** (*Internet Key Exchange v2*) — vyjednávanie kľúčov a SA (*Security Association*)

**Použitie v praxi:**
- Site-to-Site VPN (banky, pobočky) — [[Q43]] scenár 43.7
- Remote Access VPN (zamestnanci z domu)

**Šifrovacie sady:** AES-256-GCM (AEAD), ECDHE pre PFS.

---
## Spätné prepojenia
Kontext: [[Q43]]
Súvisí s: [[concepts/TLS]], [[concepts/PFS]], [[concepts/AEAD]]
