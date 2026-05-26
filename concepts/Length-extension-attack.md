---
tags: [kry, concept, topic/utoky]
---
# Length Extension Attack (Útok predĺžením správy)

**Length extension attack** je útok na Merkle-Damgård hašovacie funkcie (SHA-1, SHA-2, MD5).

**Princíp:** Útočník pozná $H(m)$ a dĺžku $m$, ale **nepozná** $m$ samotné. Napriek tomu môže vypočítať $H(m \| \text{padding} \| m')$ pre ľubovoľné $m'$.

**Prečo funguje:** Výstup Merkle-Damgård haša = interný stav po poslednom bloku. Útočník "pokračuje" v hašovaní od tohto stavu.

**Praktický dopad:** Ak API overuje `H(secret || data)`, útočník môže pridávať ľubovoľné dáta a stále dostane platný haš — bez znalosti `secret`.

**Ochrana:**
- Použiť **HMAC** (nie holý $H(k\|m)$)
- Použiť **SHA-3** (Sponge konštrukcia — imunná)
- Použiť $H(m\|k)$ namiesto $H(k\|m)$ — čiastočná ochrana

---
## Spätné prepojenia
Kontext: [[Q07]]
Súvisí s: [[concepts/Merkle-Damgard]], [[concepts/HMAC]], [[concepts/SHA-3]]
