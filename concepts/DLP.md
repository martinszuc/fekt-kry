---
tags: [kry, concept, topic/matematika]
---
# DLP — Diskrétny logaritmus (Discrete Logarithm Problem)

**DLP** je problém nájsť exponent $e$ v rovnici $c \equiv z^e \pmod{m}$, kde $c$, $z$, $m$ sú známe.

**Prečo ťažký:** Umocňovanie modulo je rýchle (Square-and-Multiply: $O(\log e)$), ale inverzia (logaritmus) je výpočtovo náročná — neexistuje subexponenciálny algoritmus pre všeobecné grupy.

**Kryptosystémy závislé na DLP:**
- Diffie-Hellman výmena kľúčov ([[concepts/Diffie-Hellman]])
- ElGamal ([[concepts/ElGamal]])
- DSA, ECDSA ([[concepts/ECDSA]]), EdDSA ([[concepts/EdDSA]])
- Schnorrov protokol ([[concepts/Schnorr]])

**ECDLP:** DLP na eliptických krivkách — ešte ťažšie; umožňuje kratšie kľúče.

**PQC hrozba:** Shorův algoritmus rieši DLP polynomiálne → DLP systémy sú kvantovo-zraniteľné.

---
## Spätné prepojenia
Detailne: [[Q23]]
Súvisí s: [[concepts/Eliptické-krivky]], [[concepts/Shorov-algoritmus]]
