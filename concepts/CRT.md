---
tags: [kry, concept, topic/matematika]
---
# CRT — Čínska veta o zvyškoch (Chinese Remainder Theorem)

**CRT** hovorí: ak sú $n_1, n_2, \ldots, n_k$ navzájom nesúdeliteľné, potom sústava kongruencií
$$x \equiv a_1 \pmod{n_1}, \quad x \equiv a_2 \pmod{n_2}, \ldots$$
má **jednoznačné riešenie** modulo $n_1 \cdot n_2 \cdots n_k$.

**Konštruktívny dôkaz:** Riešenie sa vypočíta ako $x = \sum_i a_i M_i (M_i^{-1} \bmod n_i) \bmod N$.

**Kryptografické využitie:**
1. **RSA dešifrovanie** — CRT zrýchľuje RSA dešifrovanie 4× (výpočet modulo $p$ a $q$ zvlášť).
2. **Rabinov systém** — kombinovanie odmocnín modulo $p$ a $q$ do 4 kandidátov.
3. **Hastadov útok** — rekonštrukcia $m^e$ z $e$ zvyškov po rôznych moduloch.

---
## Spätné prepojenia
Použitie: [[Q21]], [[Q31]]
Súvisí s: [[concepts/RSA]], [[concepts/Rabin]]
