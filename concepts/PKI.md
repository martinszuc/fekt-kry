---
tags: [kry, concept, topic/infrastruktura]
---
# PKI — Public Key Infrastructure

**PKI** (*Infraštruktúra verejných kľúčov*) je sústava certifikačných autorít, certifikátov a protokolov, ktorá umožňuje **dôveryhodné viazanie verejného kľúča na identitu**.

**Komponenty:**
- **CA** (*Certificate Authority*) — vydáva a podpisuje digitálne certifikáty
- **RA** (*Registration Authority*) — overuje identitu pred vydaním certifikátu
- **CRL** (*Certificate Revocation List*) — zoznam zrušených certifikátov
- **OCSP** (*Online Certificate Status Protocol*) — online overenie platnosti certifikátu
- **Certifikát X.509** — štandard formátu certifikátu ([[concepts/X.509]])

**Dôveryhodnosť:**
- Koreňová CA (*Root CA*) — zásadná dôvera, zabudovaná v OS/prehliadači
- Stredná CA (*Intermediate CA*) — vydáva certifikáty pre zákazníkov
- Certifikátový reťazec — verifikácia po koreňovú CA

**Použitie:** TLS/HTTPS, eIDAS (kvalifikovaná PKI), kódové podpisy, email (S/MIME).

---
## Spätné prepojenia
Kontext: [[Q16]], [[Q17]], [[Q18*]], [[Q42]]
Súvisí s: [[concepts/X.509]], [[concepts/eIDAS]], [[concepts/TLS]]
