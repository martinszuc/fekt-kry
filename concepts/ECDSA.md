---
tags: [kry, concept, topic/asymetria, topic/podpisy]
---
# ECDSA — Elliptic Curve Digital Signature Algorithm

**ECDSA** je štandard pre digitálny podpis na báze eliptických kriviek (FIPS 186-4). Je efektívnejšou variantou DSA.

**Základ bezpečnosti:** [[concepts/DLP]] na eliptických krivkách (ECDLP) — nájsť $k$ z $Q = kP$ je výpočtovo nemožné.

**Krivky:** NIST P-256, P-384, P-521 (najčastejšie); secp256k1 (Bitcoin).

**Podpis:** $(r, s)$ kde $r = (kG)_x \bmod n$, $s = k^{-1}(H(m) + r \cdot sk) \bmod n$.

**Slabiny:**
- Vyžaduje **dobrý CSPRNG** pre každý podpis — ak sa $k$ opakuje, privátny kľúč je kompromitovaný (PS3 incident).
- **Tvárnosť**: $(r,s)$ a $(r,-s)$ sú oba platné podpisy.

**Oprava:** [[concepts/EdDSA]] — deterministický, konštantný čas, SUF-CMA bezpečný.

---
## Spätné prepojenia
Porovnanie: [[Q35]], [[Q36]]
Matematika: [[concepts/Eliptické-krivky]], [[concepts/DLP]]
