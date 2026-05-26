---
tags: [kry, concept, topic/protokoly]
---
# PFS — Perfect Forward Secrecy

**PFS** (*Perfektné dopredu utajenie*) je vlastnosť kryptografického protokolu, pri ktorej **kompromitácia dlhodobého kľúča neodhalí minulú komunikáciu**.

**Princíp:** Pre každú reláciu sa generuje nový **dočasný (ephemeral)** kľúč. Dlhodobý kľúč (napr. certifikát servera) slúži len na autentizáciu, nie na šifrovanie dát.

**Realizácia:** Pomocou **ECDHE** (*Elliptic Curve Diffie-Hellman Ephemeral*) alebo **DHE**:
```
Každá relácia: nový (a, b) → nové spoločné tajomstvo K
Po skončení relácie: a, b sú zmazané
Kompromitácia dlhodobého kľúča servera → nič sa nedá dešifrovať z minulosti
```

**Kde je povinné:**
- **TLS 1.3** — ECDHE povinné (RSA key exchange zrušené)
- **IPsec/IKEv2** — ECDHE odporúčané
- **Signal protokol** — Double Ratchet pre PFS aj pre budúce správy

**Protiklad:** RSA key exchange (TLS 1.2) — bez PFS. Jedna kompromitácia = dešifrovanie celej histórie.

---
## Spätné prepojenia
Kontext: [[Q43]]
Súvisí s: [[concepts/Diffie-Hellman]], [[concepts/TLS]], [[concepts/IPsec]]
