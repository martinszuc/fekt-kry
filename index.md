---
tags: [kry, exam, moc]
title: MPC-KRY — Domovský list
---

# 🔐 MPC-KRY — Kryptografia, mapa otázok

> [!info] Čo je toto?
> Toto je **Obsidian vault** s mojimi študijnými poznámkami ku skúške z predmetu **MPC-KRY (Kryptografia)**. Každá skúšková otázka má vlastnú poznámku v priečinku `questions/`. Pojmy, algoritmy a skratky majú atomický stub v `concepts/`.
>
> **Legenda skratiek:** vault = trezor poznámok, MOC = Map of Content (mapa obsahu), stub = krátka stránka s definíciou a backlinkmi, PQC = Post-Quantum Cryptography, QES = Qualified Electronic Signature.

> [!tip] Ako čítať tento vault
> 1. **Graph view** (`Ctrl/Cmd+G`) — vizualizácia prepojení medzi otázkami a pojmami.
> 2. Klikni na **`[[wikilink]]`** — presmerovanie na danú poznámku.
> 3. V každej otázke nájdeš **Mermaid diagram**, **callouts** (`[!summary]`, `[!tip]`, `[!warning]`, `[!example]`) a **Flashcards** (`Q:: / A::`) pre Spaced Repetition plugin.
> 4. `Ctrl/Cmd+O` — rýchle vyhľadanie ľubovoľnej otázky alebo pojmu.

---

## 📚 Otázky podľa tematických okruhov

### 1) Základy kryptografie

- [[Q01]] — Formálna definícia kryptosystému $(P,C,K,E,D)$; symetrická vs. asymetrická šifra
- [[Q02]] — Architektúra bezpečnosti v RM OSI (ISO 7498-2): časti, implementácia
- [[Q03]] — Bezpečnostné služby (dôvernosť, integrita, auth…) a kryptografické mechanizmy
- [[Q04]] — Kroky pre zaistenie bezpečnej komunikácie (hybridné šifrovanie v praxi)
- [[Q05]] — Modely hrozieb: Destruction, Corruption, Removal, Disclosure, Interruption

### 2) Hašovacie funkcie a podpisy na hašoch

- [[Q06]] — Hašovacie funkcie: formálna definícia, vlastnosti, bezpečnosť, použitie
- [[Q07]] — Iteračné hašovacie funkcie (Merkle–Damgård): konštrukcia, požiadavky, length-extension útok
- [[Q08]] — Hubová konštrukcia (SHA-3/Keccak): absorpcia, vytláčanie, XOF (SHAKE)
- [[Q09]] — Lamportov jednorazový podpis (OTS): princíp, výhody, nevýhody
- [[Q10]] — Winternitzov podpis (WOTS): parameter $w$, kompromis veľkosť/rýchlosť

### 3) Generátory náhodných čísel

- [[Q11]] — Entropia: vzťah k bezpečnosti CSPRNG, dôsledky nedostatočnej entropie
- [[Q12]] — Požiadavky na kryptograficky bezpečné generátory (CSPRNG): predvídateľnosť, back/forward secrecy
- [[Q13]] — Príklady realizácie CSPRNG: TRNG, HMAC_DRBG, Hash_DRBG, CTR_DRBG (NIST SP 800-90A)

### 4) Kvantová kryptografia

- [[Q14]] — Hrozba kvantových počítačov: Shor (RSA, DLP), Grover (symetrika), implikácie
- [[Q15]] — QKD: dôvody, princíp, realizačné problémy, protokoly BB84, EPR, COW

### 5) Digitálne podpisy, časové razítka a eIDAS

- [[Q16]] — Digitálny podpis: formálna definícia, požiadavky, súčinnosť s hašom
- [[Q17]] — Časové razítko: účel, protokol RFC 3161, TSA, požiadavky
- [[Q18]] — eIDAS: elektronický podpis, pečať, časové razítko (prehľad)
- [[Q42]] — eIDAS právny rámec podrobne: SES / AdES / QES, QSCD, EUDI Wallet

### 6) Asymetrické systémy a útoky

- [[Q19]] — McEliece: úvod, princíp, výhody/nevýhody (detail → [[Q40]])
- [[Q20]] — ECDH nad $\mathbb{F}_p$: parametre, výpočet kľúčov, priebeh ⚠️ *zvyčajne preskakované*
- [[Q21]] — Hastadov útok na RSA s malým verejným exponentom $e$
- [[Q22]] — Slepý podpis (Blind Signature) na základe RSA: protokol, aplikácie (e-cash, voľby)
- [[Q23]] — Diskrétny logaritmus (DLP): charakteristika, systémy závislé na DLP
- [[Q24]] — Faktorizácia: problém, RSA závislosť, príklad prelomenia
- [[Q31]] — Rabinov kryptosystém: kľúče, šifrovanie $c=m^2$, dešifrovanie (CRT, 4 kandidáti)
- [[Q32]] — Schnorrov identifikačný a podpisový protokol (ZKP, Fiat–Shamirov transform)
- [[Q33]] — Slabiny raw RSA: determinizmus, malý exponent, multiplikativita
- [[Q34]] — RSA-OAEP vs. RSA-PSS: účel, princíp, porovnanie

### 7) Autentizácia a protokoly

- [[Q25]] — Faktory overenia identity (znalostný, vlastnícky, biometrický, PUF); kritériá výberu MFA
- [[Q26]] — Autentizačné protokoly: princíp, parametry čerstvosti, útoky ⚠️ *zvyčajne preskakované*

### 8) BAN logika

- [[Q27]] — BAN logika: definícia, typ (epistemická), notácia, účel ⚠️ *zvyčajne preskakované*
- [[Q28]] — BAN logika: 5 otázok, 3 typy objektov (Principals, Keys, Formulae)
- [[Q29]] — BAN logika: 3 konštrukcie (viera, videnie, čerstvosť) + 3 pravidlá (MM, NV, JR)
- [[Q30]] — BAN logika: 5 krokov analýzy protokolu (Idealizácia→Predpoklady→Ciele→Odvodzovanie→Vyhodnotenie)

### 9) Postkvantová kryptografia (PQC)

- [[Q35]] — EdDSA vs. ECDSA: deterministický nonce, Twisted Edwards krivky, PS3 incident ⚠️ *zvyčajne preskakované*
- [[Q36]] — EUF-CMA a SUF-CMA: definície, tvárnosť podpisov, Bitcoin Malleability Attack
- [[Q37]] — PQC: dôvody vzniku (Shor, Grover, SNDL), 5 rodín konštrukcií, NIST štandardy 2024
- [[Q38]] — LWE: princíp $\mathbf{b}=A\mathbf{s}+\mathbf{e}$, prečo je ťažký, Regevovo šifrovaní bitu
- [[Q39]] — LWE vs. Ring-LWE vs. Module-LWE: porovnanie, NTT, Kyber parametre
- [[Q40]] — McEliece detailne: generovanie kľúčov ($\hat{G}=SGP$), šifrovanie, dešifrovanie
- [[Q41]] — Niederreiterov kryptosystém: kontrolná matica $H$, syndróm, porovnanie s McElieceom

### 10) Ideové návrhy

- [[Q43]] — Ideové návrhy kryptosystémov: vzdialená auth, IoT, streaming, e-voľby, e-government, bankové VPN

---

## 🧭 Skúškové info

> [!summary] Formát skúšky
> - **5 otázok** za **60 minút** → ~12 min/otázka
> - **60 bodov** celkovo
> - **Vždy minimálne 1× Ideový návrh** → [[Q43]] — dobre sa nauč všetky scenáre!
> - Zvyčajne preskakované: Q20, Q26, Q27, Q35 — sú tu pre kontext, nie pre skúšku

> [!tip] Stratégia štúdia
> **Povinné (zvyčajne na skúške):** Q01–Q19, Q21–Q25, Q28–Q34, Q36–Q43
> **Voliteľné (skúška preskakuje):** Q20, Q26, Q27, Q35
> **Vždy sa opakuje:** Q43 (Ideový návrh) — nauč sa aspoň 4 scenáre spamäti

---

## 🧩 Concept index

### Algoritmy a primitíva
[[concepts/AES]] · [[concepts/DES]] · [[concepts/ChaCha20]] · [[concepts/RSA]] · [[concepts/ElGamal]] · [[concepts/ECDH]] · [[concepts/ECDSA]] · [[concepts/EdDSA]] · [[concepts/Schnorr]] · [[concepts/Rabin]] · [[concepts/Diffie-Hellman]]

### Hašovacie funkcie
[[concepts/SHA-2]] · [[concepts/SHA-3]] · [[concepts/HMAC]] · [[concepts/MAC]] · [[concepts/AEAD]]

### Konštrukcie
[[concepts/Merkle-Damgard]] · [[concepts/Sponge-construction]] · [[concepts/OAEP]] · [[concepts/PSS]]

### Postkvantová kryptografia
[[concepts/LWE]] · [[concepts/Kyber]] · [[concepts/Dilithium]] · [[concepts/SPHINCS+]] · [[concepts/McEliece]] · [[concepts/Niederreiter]] · [[concepts/Goppa-kod]] · [[concepts/Mriežková-kryptografia]]

### Matematické pojmy
[[concepts/DLP]] · [[concepts/Faktorizacia]] · [[concepts/CRT]] · [[concepts/Eulerova-funkcia]] · [[concepts/Eliptické-krivky]] · [[concepts/Trapdoor-funkcia]]

### Útoky
[[concepts/Birthday-attack]] · [[concepts/Length-extension-attack]] · [[concepts/Replay-attack]] · [[concepts/MitM]] · [[concepts/Side-channel]]

### Štandardy a normy
[[concepts/eIDAS]] · [[concepts/PKI]] · [[concepts/TLS]] · [[concepts/IPsec]] · [[concepts/X.509]] · [[concepts/FIPS-140]] · [[concepts/NIST-SP-800-90A]] · [[concepts/RFC-3161]]

### Kvantová kryptografia
[[concepts/QKD]] · [[concepts/BB84]] · [[concepts/Shorov-algoritmus]] · [[concepts/Groverov-algoritmus]] · [[concepts/No-cloning-teorem]]

### Autentizácia a identita
[[concepts/BAN-logika]] · [[concepts/Nonce]] · [[concepts/MFA]] · [[concepts/PFS]] · [[concepts/Zero-Knowledge]]

### Základné pojmy
[[concepts/Kryptosystém]] · [[concepts/Symetrická-šifra]] · [[concepts/Asymetrická-šifra]]

---

## 🔤 Slovník hlavných skratiek

| Skratka | Plné znenie | Kde |
|---------|------------|-----|
| **AES** | Advanced Encryption Standard | [[concepts/AES]] |
| **RSA** | Rivest–Shamir–Adleman | [[concepts/RSA]] |
| **ECC** | Elliptic Curve Cryptography | [[concepts/Eliptické-krivky]] |
| **ECDH** | Elliptic Curve Diffie–Hellman | [[concepts/ECDH]] · [[Q20]] |
| **ECDSA** | EC Digital Signature Algorithm | [[concepts/ECDSA]] · [[Q35]] |
| **EdDSA** | Edwards-curve DSA (napr. Ed25519) | [[concepts/EdDSA]] · [[Q35]] |
| **HMAC** | Hash-based MAC | [[concepts/HMAC]] |
| **MAC** | Message Authentication Code | [[concepts/MAC]] |
| **AEAD** | Authenticated Encryption with Associated Data | [[concepts/AEAD]] |
| **XOF** | Extendable-Output Function (napr. SHAKE128/256) | [[Q08]] · [[concepts/SHA-3]] |
| **OTS** | One-Time Signature (jednorazový podpis) | [[Q09]] |
| **WOTS** | Winternitz OTS | [[Q10]] |
| **CSPRNG** | Cryptographically Secure Pseudo-RNG | [[Q12]] |
| **TRNG** | True RNG — hardvérový zdroj entropie | [[Q13]] |
| **DRBG** | Deterministic Random Bit Generator | [[Q13]] · [[concepts/NIST-SP-800-90A]] |
| **QKD** | Quantum Key Distribution | [[concepts/QKD]] · [[Q15]] |
| **BB84** | Bennett–Brassard 1984 QKD protokol | [[concepts/BB84]] · [[Q15]] |
| **TSA** | Time Stamping Authority | [[Q17]] · [[concepts/RFC-3161]] |
| **eIDAS** | EU nariadenie 910/2014 o el. identifikácii | [[concepts/eIDAS]] · [[Q18]] · [[Q42]] |
| **SES / AdES / QES** | Simple / Advanced / Qualified Electronic Signature | [[Q18]] · [[Q42]] |
| **QSCD** | Qualified Signature Creation Device (HSM, čipová karta) | [[Q42]] |
| **EUDI Wallet** | European Digital Identity Wallet (eIDAS 2.0, 2026) | [[Q42]] |
| **DLP** | Discrete Logarithm Problem | [[concepts/DLP]] · [[Q23]] |
| **CRT** | Chinese Remainder Theorem (Čínska veta o zvyškoch) | [[concepts/CRT]] · [[Q21]] · [[Q31]] |
| **CCA2** | Chosen Ciphertext Attack (adaptívny) | [[Q34]] |
| **EUF-CMA** | Existential Unforgeability under Chosen Message Attack | [[Q36]] |
| **SUF-CMA** | Strong Existential Unforgeability under CMA | [[Q36]] |
| **OAEP** | Optimal Asymmetric Encryption Padding | [[concepts/OAEP]] · [[Q34]] |
| **PSS** | Probabilistic Signature Scheme | [[concepts/PSS]] · [[Q34]] |
| **MFA** | Multi-Factor Authentication | [[concepts/MFA]] · [[Q25]] |
| **PUF** | Physical Unclonable Function | [[Q25]] |
| **MitM** | Man-in-the-Middle attack | [[concepts/MitM]] · [[Q26]] |
| **PQC** | Post-Quantum Cryptography | [[Q37]] |
| **LWE** | Learning With Errors | [[concepts/LWE]] · [[Q38]] · [[Q39]] |
| **NTT** | Number Theoretic Transform (rýchle násobenie polynómov) | [[Q39]] |
| **PFS** | Perfect Forward Secrecy | [[concepts/PFS]] · [[Q43]] |
| **HSM** | Hardware Security Module | [[Q17]] · [[Q18]] |
| **BAN** | Burrows–Abadi–Needham logika | [[concepts/BAN-logika]] · [[Q27]]–[[Q30]] |
| **ZKP** | Zero-Knowledge Proof | [[concepts/Zero-Knowledge]] · [[Q32]] |
| **SNDL** | Store Now, Decrypt Later (PQC hrozba) | [[Q37]] |
| **KEM** | Key Encapsulation Mechanism (napr. Kyber) | [[concepts/Kyber]] · [[Q37]] |
| **SVP** | Shortest Vector Problem (mriežkový problém) | [[Q38]] · [[concepts/LWE]] |

---

## ⚙️ Technické tipy pre Obsidian

> [!tip] Odporúčané pluginy
> - **Spaced Repetition** — flashcards `Q:: / A::` v každej poznámke Q01–Q43
> - **Mermaid** (zabudovaný) — diagramy `flowchart`, `sequenceDiagram`, `quadrantChart`
> - **Callout** (zabudovaný) — `[!summary]`, `[!tip]`, `[!warning]`, `[!example]`
> - **Graph view** — zobrazí sieť prepojení; otázky sú prepojené cez `[[wikilinks]]`

> [!warning] LaTeX vzorce
> Matematika je v `$...$` (inline) alebo `$$...$$` (blok). Pre správne zobrazenie v Obsidian: `Settings → Editor → zapni "Render math in live preview"`.

> [!tip] Rýchla navigácia
> - `Ctrl+O` — Quick Open (otvoriť ľubovoľnú poznámku)
> - `Ctrl+G` — Graph view
> - `Ctrl+Shift+F` — globálne vyhľadávanie
> - `Alt+←/→` — späť/dopredu v histórii
