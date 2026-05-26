---
tags: [kry, concept, topic/utoky]
---
# MitM — Man-in-the-Middle Attack (Útok prostredníkom)

**MitM útok**: útočník sa vkladá medzi dvoch komunikujúcich účastníkov, odpočúva a prípadne modifikuje ich komunikáciu, pričom Alice verí, že hovorí s Bobom a naopak.

**Schéma:**
```
Alice ←→ [Útočník Eva] ←→ Bob
Alice si myslí, že hovorí s Bobom
Bob si myslí, že hovorí s Alicou
Eva vidí a môže meniť všetku komunikáciu
```

**Typicky útočí na:** Diffie-Hellman výmenu kľúčov bez autentizácie — každá strana dohodne kľúč s útočníkom, nie medzi sebou.

**Ochrana:**
- **PKI certifikáty** — verejné kľúče podpísané dôveryhodnou CA
- **Digitálne podpisy** pri výmene kľúčov
- **TOFU** (*Trust On First Use*) — SSH fingerprint

---
## Spätné prepojenia
Kontext: [[Q26]]
Súvisí s: [[concepts/PKI]], [[concepts/Diffie-Hellman]]
