---
tags: [kry, concept, topic/utoky]
---
# Side-channel Attack (Útok postranným kanálom)

**Side-channel útok** nevyužíva matematickú slabinu algoritmu, ale **fyzické meranie** pri jeho vykonávaní — čas, spotrebu energie, elektromagnetické vyžarovanie, zvuk.

**Typy:**
| Typ | Čo meria | Príklad |
|-----|---------|---------|
| **Timing attack** | Čas výpočtu | RSA modulárne umocňovanie závisí na tajnom kľúči |
| **Power analysis** | Spotrebu energie | SPA/DPA útok na čipové karty |
| **EM attack** | Elektromagnetické pole | Čítanie šifrovaného disku z diaľky |
| **Acoustic attack** | Zvuk pri výpočte | Rekonštrukcia kľúča z hluku notebooku |

**Obrana:**
- Konštantný čas výpočtu (*constant-time implementations*)
- Pridávanie náhodného šumu k operáciám (*blinding*)
- Fyzická ochrana hardvéru (Faradayova klietka)

**ECDSA je zraniteľná** ak implementácia nie je opatrná. **EdDSA** ([[concepts/EdDSA]]) je navrhnutá odolne.

---
## Spätné prepojenia
Kontext: [[Q35]]
Súvisí s: [[concepts/EdDSA]], [[concepts/ECDSA]]
