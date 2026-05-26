---
tags: [kry, concept, topic/kvantova, topic/utoky]
---
# Shorův algoritmus

**Shorův algoritmus** (Peter Shor, 1994) je kvantový algoritmus riešiaci **faktorizáciu** a **diskrétny logaritmus** v **polynomiálnom čase**.

**Dopad na kryptografiu:**
| Systém | Základ bezpečnosti | Po Shorovi |
|--------|-------------------|-----------|
| RSA | Faktorizácia | ❌ Prelomený |
| DH, DSA | DLP mod p | ❌ Prelomený |
| ECDSA, EdDSA | ECDLP | ❌ Prelomený |

**Princíp:** Využíva **kvantovú Fourierovu transformáciu** na nájdenie periódy funkcie $f(x) = a^x \bmod n$, z ktorej sa faktorizácia odvodí klasicky.

**Hardvérové požiadavky:** Pre RSA-2048 potrebuje ~4000 logických qubitov + milióny fyzických qubitov (kvantová korekcia chýb). Aktuálne počítače majú ~100–1000 nespoľahlivých qubitov.

**Záver:** Dnes nie je k dispozícii, ale hrozba je dostatočná na migráciu na PQC už teraz.

---
## Spätné prepojenia
Kontext: [[Q14]], [[Q37]]
Súvisí s: [[concepts/Faktorizacia]], [[concepts/DLP]], [[concepts/Groverov-algoritmus]]
