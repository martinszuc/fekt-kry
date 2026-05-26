---
tags: [kry, concept, topic/utoky]
---
# Birthday Attack (Útok narodeninového paradoxu)

**Birthday attack** využíva **narodeninový paradox** štatistiky na hľadanie kolízií v hašovacích funkciách.

**Narodeninový paradox:** V skupine $\sqrt{N}$ ľudí je pravdepodobnosť spoločných narodenín >50%. Analogicky: na nájdenie kolízie $H(x) = H(y)$ v $n$-bitovom haši stačí $2^{n/2}$ pokusov, nie $2^n$.

**Dôsledok pre bezpečnosť:**
- 128-bitový haš → 64-bit kolízna odolnosť (útok v $2^{64}$ krokoch — príliš málo!)
- SHA-256 → 128-bit kolízna odolnosť → bezpečné

**Preto:** Pre 128-bit kolíznu bezpečnosť potrebujeme **256-bitový haš**.

**Použitie útočníkom:** Nájsť dve rôzne správy $m_1 \neq m_2$ kde $H(m_1) = H(m_2)$ — umožňuje podvrhnutie podpisu.

---
## Spätné prepojenia
Kontext: [[Q06]], [[Q07]]
Súvisí s: [[concepts/SHA-2]], [[concepts/SHA-3]]
