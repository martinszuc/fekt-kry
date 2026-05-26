---
tags: [kry, concept, topic/asymetria, topic/podpisy]
---
# Schnorrov protokol a podpis

**Schnorrov protokol** (Claus-Peter Schnorr, 1989) je identifikačný a podpisový protokol na báze [[concepts/DLP]].

**Základ:** Nulové-znalostný dôkaz (Zero-Knowledge Proof) znalosti diskrétneho logaritmu.

**3 kroky identifikácie:** Záväzok ($r = g^k$) → Výzva ($e$) → Odpoveď ($z = k + ex$).

**Podpis:** Fiat-Shamirov transform — výzva $e = H(m \| r)$ namiesto interaktívneho Boba.

**Výhody:** Krátke podpisy, dokazateľná bezpečnosť, agregácia podpisov (MuSig).

**Dedičstvo:** EdDSA ([[concepts/EdDSA]]) je priamo odvodená od Schnorra na Twisted Edwards krivkách.

---
## Spätné prepojenia
Detailne: [[Q32]]
Súvisí s: [[concepts/DLP]], [[concepts/EdDSA]], [[concepts/Zero-Knowledge]]
