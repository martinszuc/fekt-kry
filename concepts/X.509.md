---
tags: [kry, concept, topic/infrastruktura]
---
# X.509 — štandard digitálnych certifikátov

**X.509** je medzinárodný štandard (ITU-T) pre formát digitálnych certifikátov verejného kľúča. Je základom PKI.

**Čo obsahuje certifikát:**
- Identita subjektu (meno, organizácia, doménové meno)
- **Verejný kľúč** subjektu
- Digitálny podpis CA
- Platnosť (od–do)
- Sériové číslo, rozšírenia (SAN, EKU, CRL endpoint…)

**Verzia:** X.509 v3 je aktuálna (s rozšíreniami).

**Kódovanie:** DER (binárne), PEM (Base64 zakódované).

**Reťazec dôvery:** Certifikát → Stredná CA → Koreňová CA (uložená v OS).

**Typy certifikátov:**
- **DV** (*Domain Validated*) — overenie len domény
- **OV** (*Organization Validated*) — overenie organizácie
- **EV** (*Extended Validation*) — striktné overenie

---
## Spätné prepojenia
Kontext: [[Q16]], [[Q17]], [[Q42]]
Súvisí s: [[concepts/PKI]], [[concepts/eIDAS]]
