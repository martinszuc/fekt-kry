---
tags: [kry, concept, topic/asymetria, topic/podpisy]
---
# EdDSA — Edwards-curve Digital Signature Algorithm

**EdDSA** je moderný digitálny podpis na Twisted Edwards krivkách, navrhnutý Bernsteinom a spol. (RFC 8032).

**Najčastejšia inštancia: Ed25519** (Curve25519, ~128-bit bezpečnosť).

**Kľúčové vlastnosti:**
- **Deterministický**: nonce $r = H(sk_2 \| m)$ — bez potreby externého RNG
- **Konštantný čas**: odolný voči side-channel útokom
- **SUF-CMA bezpečný**: bez tvárnosti podpisov ([[Q36]])
- **Rýchly**: batch verifikácia viacerých podpisov naraz

**Porovnanie s ECDSA:** Pozri [[Q35]].

**Použitie:** SSH kľúče (OpenSSH), TLS certifikáty, Signal protokol, Monero.

---
## Spätné prepojenia
Detailne: [[Q35]], [[Q36]]
Súvisí s: [[concepts/ECDSA]], [[concepts/Schnorr]], [[concepts/Eliptické-krivky]]
