---
tags: [kry, concept, topic/zaklady]
---
# Kryptosystém

**Kryptosystém** je formálne definovaný ako **usporiadaná pätica** $\mathcal{K} = (P, C, K, E, D)$:

- $P$ — množina otvorených textov (*plaintextov*)
- $C$ — množina šifrových textov (*ciphertextov*)
- $K$ — množina kľúčov (*kľúčový priestor*)
- $E$ — množina šifrovacích funkcií $e_k: P \to C$
- $D$ — množina dešifrovacích funkcií $d_k: C \to P$

**Požiadavka korektnosti:** $\forall k \in K, \forall m \in P: d_k(e_k(m)) = m$

**Typy kryptosystémov:**
- **Symetrický** — $k_e = k_d$ (jeden zdieľaný kľúč)
- **Asymetrický** — $k_e \neq k_d$ (pár verejný/súkromný)

---
## Spätné prepojenia
Detailne: [[Q01]]
Súvisí s: [[concepts/Symetrická-šifra]], [[concepts/Asymetrická-šifra]]
