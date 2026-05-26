---
tags: [kry, concept, topic/pqc, topic/kodova]
---
# McElieceov kryptosystém

**McElieceov kryptosystém** (Robert McEliece, 1978) je najstarší asymetrický systém odolný voči kvantovým počítačom. Patrí do kódovej rodiny PQC.

**Základ bezpečnosti:** NP-ťažkosť dekódovania obecného lineárneho kódu.

**Kľúčový nápad:** Skry štruktúru Goppa kódu (efektívne dekódovateľného) za náhodne vyzerajúcu verejnú maticu pomocou maskovanej $\hat{G} = S \cdot G \cdot P$.

**Verejný kľúč:** $(\hat{G}, t)$ — veľký (stovky KB–MB).
**Súkromný kľúč:** $(S, G, P)$ a Goppa dekodér.

**Status:** NIST alternatívny PQC štandard (Classic McEliece).

---
## Spätné prepojenia
Úvod: [[Q19]], Detailne: [[Q40]], Duálna varianta: [[Q41]]
Súvisí s: [[concepts/Goppa-kod]], [[concepts/Niederreiter]]
