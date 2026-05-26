---
tags: [kry, concept, topic/asymetria]
---
# Diffie–Hellman (DH) — protokol výmeny kľúčov

**Diffie–Hellman** (1976) je prvý verejne publikovaný protokol na výmenu tajného kľúča cez nezabezpečený kanál.

**Základ bezpečnosti:** [[concepts/DLP]] — z $g^a \bmod p$ nemožno zistiť $a$.

**Priebeh:**
1. Verejné: prvočíslo $p$, generátor $g$.
2. Alice: $a \leftarrow \text{random}$, pošle $A = g^a \bmod p$.
3. Bob: $b \leftarrow \text{random}$, pošle $B = g^b \bmod p$.
4. Zdieľané tajomstvo: $K = B^a = A^b = g^{ab} \bmod p$.

**Varianty:**
- **DHE** — Ephemeral DH (dočasné kľúče; PFS)
- **ECDH** — DH na eliptických krivkách ([[Q20]])
- **ECDHE** — Ephemeral ECDH (TLS 1.3 štandard)
- **X25519** — ECDH na Curve25519 (odporúčaný)

**PQC hrozba:** Shorův algoritmus rieši DLP → [[Q37]].

---
## Spätné prepojenia
Kontext: [[Q01]], [[Q20]]
Súvisí s: [[concepts/DLP]], [[concepts/Eliptické-krivky]], [[concepts/PFS]]
