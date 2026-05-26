---
tags: [kry, concept, topic/matematika]
---
# Eulerova funkcia $\varphi(n)$

**Eulerova funkcia** (Euler's totient function) $\varphi(n)$ udáva počet celých čísel v rozsahu $[1, n]$, ktoré sú nesúdeliteľné s $n$ (t.j. $\gcd(k, n) = 1$).

**Kľúčové hodnoty:**
- Pre prvočíslo $p$: $\varphi(p) = p-1$
- Pre súčin dvoch prvočísel $n = pq$: $\varphi(n) = (p-1)(q-1)$

**Použitie v RSA:**
Pri generovaní RSA kľúčov sa vypočíta $\varphi(n) = (p-1)(q-1)$. Súkromný exponent $d$ sa nájde ako:
$$d \equiv e^{-1} \pmod{\varphi(n)}$$
Znalosť $\varphi(n)$ umožňuje výpočet $d$ — preto musí ostať tajná.

**Eulerova veta:** $a^{\varphi(n)} \equiv 1 \pmod{n}$ pre $\gcd(a,n)=1$.

---
## Spätné prepojenia
Použitie: [[Q24]], [[Q33]]
Súvisí s: [[concepts/RSA]], [[concepts/Faktorizacia]]
