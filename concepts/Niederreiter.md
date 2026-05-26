---
tags: [kry, concept, topic/pqc, topic/kodova]
---
# Niederreiterov kryptosystém

**Niederreiterov kryptosystém** (Harald Niederreiter, 1986) je duálnou variantou [[concepts/McEliece]] — využíva kontrolnú (*parity-check*) maticu $H$ namiesto generujúcej matice $G$.

**Kľúčový rozdiel:** Správa = chybový vektor váhy $t$; šifrový text = syndróm $\mathbf{c} = \hat{H}\mathbf{e}^T$.

**Výhoda:** Kratší šifrový text ($n-k$ bitov vs. $n$ bitov u McEliece).

**Bezpečnostná ekvivalencia:** Oba systémy sú považované za ekvivalentné.

**CFS podpis:** Niederreiter je základ Courtois-Finiasz-Sendrier digitálneho podpisu.

---
## Spätné prepojenia
Detailne: [[Q41]], Príbuzný: [[Q40]]
Súvisí s: [[concepts/McEliece]], [[concepts/Goppa-kod]]
