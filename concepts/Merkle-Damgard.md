---
tags: [kry, concept, topic/has]
---
# Merkle–Damgård konštrukcia

**Merkle–Damgård** je metóda stavby hašovacích funkcií ľubovoľnej dĺžky zo **kompresnej funkcie** fixnej dĺžky.

**Princíp:**
1. Správa sa doplní (*padding*) na násobok veľkosti bloku.
2. Iteratívne sa aplikuje kompresná funkcia $f$: $H_i = f(H_{i-1}, M_i)$
3. Výsledok posledného bloku je haš.

**Inicializačný vektor (IV):** Fixná hodnota $H_0$ = štandardizovaná konštanta.

**Slabina — Length Extension Attack:**
Útočník pozná $H(m)$ a môže vypočítať $H(m \| \text{padding} \| m')$ bez znalosti $m$. Preto HMAC namiesto $H(k \| m)$!

**Algoritmy:** SHA-1, SHA-2 (SHA-256, SHA-512), MD5 — všetky používajú Merkle-Damgård.

**Nástupca:** [[concepts/Sponge-construction]] (SHA-3) — odolná voči length extension.

---
## Spätné prepojenia
Detailne: [[Q07]]
Súvisí s: [[concepts/SHA-2]], [[concepts/Sponge-construction]], [[concepts/Length-extension-attack]]
