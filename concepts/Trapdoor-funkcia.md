---
tags: [kry, concept, topic/matematika]
---
# Trapdoor funkcia (jednosmerná funkcia s padacími dvierkami)

**Trapdoor one-way function** je funkcia $f$, ktorá:
1. Je ľahko vypočítateľná v dopredu smere: $y = f(x)$ — rýchle
2. Je výpočtovo nemožné invertovať bez špeciálnej znalosti (trapdoor): $x = f^{-1}(y)$ — ťažké
3. S "padacími dvierkami" (trapdoor info = súkromný kľúč) je inverzia ľahká

**Príklady v kryptografii:**
| Funkcia | Trapdoor | Základ |
|---------|---------|--------|
| $c = m^e \bmod n$ (RSA) | $(p, q)$ — faktorizácia $n$ | [[concepts/Faktorizacia]] |
| $y = g^x \bmod p$ (DH/DSA) | $x$ — diskrétny logaritmus | [[concepts/DLP]] |
| $Q = kP$ (ECC) | $k$ — skalárny násobok | [[concepts/Eliptické-krivky]] |

**Asymetrická kryptografia** stojí celá na trapdoor funkciách — verejný kľúč je smer "dopredu", súkromný kľúč je trapdoor.

---
## Spätné prepojenia
Kontext: [[Q01]], [[Q24]]
Súvisí s: [[concepts/Asymetrická-šifra]], [[concepts/DLP]], [[concepts/Faktorizacia]]
