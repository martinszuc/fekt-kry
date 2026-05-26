---
tags: [kry, concept, topic/integrita]
---
# HMAC — Hash-based Message Authentication Code

**HMAC** je štruktúra pre **MAC** (kód autentizácie správy) postavená na hašovacej funkcii. Štandard: RFC 2104, FIPS 198.

**Konštrukcia:**
$$\text{HMAC}(K, m) = H\bigl((K' \oplus \text{opad}) \| H((K' \oplus \text{ipad}) \| m)\bigr)$$
kde `ipad = 0x36...36`, `opad = 0x5C...5C` a $K'$ je kľúč doplnený/skrátený na veľkosť bloku $H$.

**Prečo nie holý $H(K\|m)$?** Kvôli *length extension attack* na Merkle-Damgård hašoch (SHA-256). HMAC tejto zraniteľnosti odolá.

**Bezpečnosť:** HMAC-SHA256 je bezpečné, pokiaľ je SHA-256 odolné voči kolíziám.

**Použitie:** TLS (MAC v record layer), JWT tokeny, TOTP/HOTP, API autentizácia.

---
## Spätné prepojenia
Kontext: [[Q06]], [[Q07]]
Súvisí s: [[concepts/MAC]], [[concepts/SHA-2]], [[concepts/SHA-3]]
