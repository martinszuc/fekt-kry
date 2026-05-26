---
tags: [kry, concept, topic/podpisy, topic/autentizacia]
---
# Zero-Knowledge Proof (Nulové-znalostný dôkaz)

**Zero-Knowledge Proof (ZKP)** je kryptografický protokol, pri ktorom môže *Prover* (dokazujúci) presvedčiť *Verifier* (overovateľa) o pravdivosti tvrdenia **bez odhalenia žiadnej ďalšej informácie** okrem samotnej pravdivosti.

**Tri vlastnosti ZKP:**
1. **Úplnosť** — ak je tvrdenie pravdivé, čestný Prover presvedčí Verifier.
2. **Spoľahlivosť** — podvodný Prover nemôže presvedčiť Verifier o nepravdivom tvrdení (okrem zanedbateľnej pravdepodobnosti).
3. **Nulová znalosti** — Verifier sa nedozvie nič okrem toho, že tvrdenie je pravdivé.

**Príklady ZKP:**
- **Schnorrov protokol** ([[Q32]]) — dôkaz znalosti diskrétneho logaritmu
- **Pedersen commitment** — záväzok k hodnote bez jej odhalenia
- **zk-SNARK/zk-STARK** — efektívne ZKP systémy (Zcash, Ethereum)

**Použitie:**
- E-voľby — dôkaz, že hlas je v {0,1} bez odhalenia hodnoty ([[Q43]])
- Anonymné credentials — dôkaz atribútu (vek > 18) bez odhalenia dátumu narodenia

---
## Spätné prepojenia
Kontext: [[Q32]], [[Q43]]
Súvisí s: [[concepts/Schnorr]], [[concepts/BAN-logika]]
