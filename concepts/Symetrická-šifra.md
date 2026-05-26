---
tags: [kry, concept, topic/zaklady]
---
# Symetrická šifra

**Symetrická šifra** je kryptosystém, kde šifrovací kľúč $k_e$ a dešifrovací kľúč $k_d$ sú **identické** (alebo sa jeden ľahko odvodí z druhého): $k_e = k_d = k$.

**Typy:**
- **Bloková šifra** — šifruje bloky fixnej dĺžky; [[concepts/AES]], [[concepts/DES]]
- **Prúdová šifra** — generuje kľúčový prúd XOR-ovaný s plaintextom; [[concepts/ChaCha20]]

**Výhody:** Veľmi rýchla (Gbit/s); krátke kľúče (128–256 bit).
**Nevýhody:** Nutnosť bezpečnej distribúcie zdieľaného kľúča (*key distribution problem*).

**Riešenie distribúcie:** Použiť asymetrickú kryptografiu na výmenu symetrického kľúča (hybridné šifrovanie).

---
## Spätné prepojenia
Kontext: [[Q01]]
Súvisí s: [[concepts/AES]], [[concepts/ChaCha20]], [[concepts/Asymetrická-šifra]]
