---
tags: [kry, concept, topic/zaklady]
---
# Asymetrická šifra (Kryptografia s verejným kľúčom)

**Asymetrická šifra** je kryptosystém, kde existujú **dva rôzne kľúče**: verejný $pk$ a súkromný $sk$, pričom $pk$ nemožno v reálnom čase vypočítať zo znalosti $sk^{-1}$ (a naopak).

- **Verejný kľúč** $pk$ — voľne dostupný; šifruje alebo overuje podpis
- **Súkromný kľúč** $sk$ — utajený; dešifruje alebo podpisuje

**Základ bezpečnosti:** Jednosmerné funkcie s padacími dvierkami (*trapdoor one-way functions*) — [[concepts/Trapdoor-funkcia]].

**Nevýhody:** Pomalá (~1000× pomalšia ako symetrika); dlhé kľúče.

**Príklady:** [[concepts/RSA]], [[concepts/ElGamal]], [[concepts/ECDSA]], [[concepts/EdDSA]].

**Hybridné šifrovanie:** Asymetrika vymení symetrický kľúč → symetrika šifruje dáta.

---
## Spätné prepojenia
Kontext: [[Q01]]
Súvisí s: [[concepts/RSA]], [[concepts/Trapdoor-funkcia]], [[concepts/Symetrická-šifra]]
