---
tags: [kry, concept, topic/matematika, topic/asymetria]
---
# Eliptické krivky (ECC — Elliptic Curve Cryptography)

**Eliptická krivka** nad poľom $\mathbb{F}_p$ je množina bodov spĺňajúcich rovnicu Weierstrassovej formy:
$$y^2 \equiv x^3 + ax + b \pmod{p}$$
plus špeciálny „bod v nekonečne" $\mathcal{O}$ (neutrálny prvok grupy).

**Grupová operácia:** Sčítanie bodov na krivke — geometricky: priamka pretne krivku v troch bodoch, tretí bod zrkadlovo odrazi.

**Bezpečnosť:** ECDLP — nájsť $k$ z $Q = kP$ (násobenie bodu skalárom). Oveľa ťažšie ako DLP nad $\mathbb{Z}_p$ → kratšie kľúče pre rovnakú bezpečnosť.

**Porovnanie kľúčov:**
| ECC | RSA | Bezpečnosť |
|-----|-----|-----------|
| 256 bit | 3072 bit | 128-bit |
| 384 bit | 7680 bit | 192-bit |

**Krivky:** NIST P-256/384/521 (Weierstrass), Curve25519 (Montgomery), Ed25519 (Twisted Edwards).

**Algoritmy:** ECDH ([[Q20]]), ECDSA ([[concepts/ECDSA]]), EdDSA ([[concepts/EdDSA]]).

---
## Spätné prepojenia
Použitie: [[Q20]], [[Q23]], [[Q32]], [[Q35]]
Súvisí s: [[concepts/DLP]], [[concepts/ECDSA]], [[concepts/EdDSA]]
