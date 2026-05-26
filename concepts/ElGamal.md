---
tags: [kry, concept, topic/asymetria]
---
# ElGamal — asymetrický kryptosystém

**ElGamal** je asymetrický šifrovací systém a systém pre digitálne podpisy navrhnutý Taherom ElGamalom (1985).

**Základ bezpečnosti:** [[concepts/DLP]] — z $g^x \bmod p$ nemožno zistiť $x$.

**Kľúče:** Súkromný $x$; verejný $y = g^x \bmod p$.

**Šifrovanie:**
1. Alice zvolí náhodné $k$, vypočíta $c_1 = g^k$, $c_2 = m \cdot y^k$.
2. Šifrový text: $(c_1, c_2)$ — dvakrát dlhší ako správa!

**Dešifrovanie:** $m = c_2 / c_1^x = m \cdot y^k / g^{kx} = m$.

**Homomorfnosť:** $\text{Enc}(m_1) \cdot \text{Enc}(m_2) = \text{Enc}(m_1 \cdot m_2)$ — využíva sa v homomorfnom šifrovaní.

**Použitie:** Základ pre Schnorr podpis, e-voľby (Paillier je modernejší).

---
## Spätné prepojenia
Kontext: [[Q01]], [[Q23]]
Súvisí s: [[concepts/DLP]], [[concepts/Schnorr]]
