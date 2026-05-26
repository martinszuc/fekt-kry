---
tags: [kry, concept, topic/autentizacia]
---
# MFA — Multi-Factor Authentication

**MFA** (*Viacfaktorová autentizácia*) vyžaduje na overenie identity overenie **dvoch alebo viacerých rôznych faktorov** z rôznych kategórií.

**Tri základné faktory:**
| Faktor | Čo je | Príklady |
|--------|-------|---------|
| **„Čo vieš"** | Znalostný | Heslo, PIN, bezpečnostná otázka |
| **„Čo máš"** | Vlastnícky | TOTP (Google Authenticator), SMS, čipová karta, hardvérový kľúč (YubiKey) |
| **„Čo si"** | Biometrický | Otisk prstu, FaceID, geometria duhovky |

**Prečo MFA?**
- Kompromitácia jedného faktora (napr. uniknuté heslo) nestačí na prihlásenie.
- NIST SP 800-63 odporúča MFA pre všetky systémy s citlivými dátami.

**2FA** = špeciálny prípad MFA s dvomi faktormi.

**Moderné varianty:** FIDO2/WebAuthn — štandard pre bezheslové prihlásenie s hardware kľúčom.

---
## Spätné prepojenia
Detailne: [[Q25]]
Súvisí s: [[concepts/Nonce]]
