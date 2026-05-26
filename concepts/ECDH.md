---
tags: [kry, concept, topic/asymetria]
---
# ECDH — Elliptic Curve Diffie–Hellman

**ECDH** je varianta Diffie-Hellman výmeny kľúčov na **eliptických krivkách**. Bezpečnosť stojí na ECDLP (Elliptic Curve Discrete Logarithm Problem).

**Princíp:**
1. Verejné parametre: krivka $E$, generátor $G$.
2. Alice: $a \leftarrow \text{random}$; verejný kľúč $A = aG$.
3. Bob: $b \leftarrow \text{random}$; verejný kľúč $B = bG$.
4. Zdieľané tajomstvo: $K = aB = bA = abG$ (obaja vypočítajú to isté).

**Varianty:**
- **ECDH** — statický (dlhodobé kľúče; bez PFS)
- **ECDHE** — ephemeral (dočasné kľúče; **PFS**; štandard v TLS 1.3)
- **X25519** — ECDHE na Curve25519 (odporúčaný, konštantný čas)

**Krivky:** Curve25519 (odporúčaná), P-256/384 (NIST; kompatibilita).

**Využitie:** TLS 1.3 key exchange, Signal protokol, WireGuard, SSH.

---
## Spätné prepojenia
Detailne: [[Q20]]
Súvisí s: [[concepts/Eliptické-krivky]], [[concepts/Diffie-Hellman]], [[concepts/PFS]]
