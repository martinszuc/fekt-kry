---
tags: [kry, exam, moc]
title: MPC-KRY — Domovský list
---

# 🔐 MPC-KRY — Kryptografia, mapa otázok

> [!info] Čo je toto?
> Toto je **Obsidian vault** s mojimi študijnými poznámkami ku skúške z predmetu **MPC-KRY (Kryptografia)**. Každá skúšková otázka má vlastnú poznámku v priečinku `questions/`. Pojmy, algoritmy a skratky majú svoj atomický „concept" stub v `concepts/`.
>
> **Skratky:** vault = trezor poznámok, MOC = Map of Content (mapa obsahu), stub = krátka stránka s definíciou a backlinkmi.

> [!tip] Ako čítať tento vault
> 1. Otvor si **Graph view** (Ctrl/Cmd+G) – uvidíš, ako sú otázky vzájomne prepojené.
> 2. Klikni na ľubovoľný `[[wikilink]]` – Obsidian ťa prenesie na danú poznámku.
> 3. V každej otázke nájdeš **Mermaid diagram**, **callouts** (žlté/zelené boxy) a **Flashcards** kompatibilné s pluginom *Spaced Repetition*.
> 4. Použi `Ctrl/Cmd+O` na rýchle vyhľadanie ľubovoľnej otázky alebo pojmu.

---

## 📚 Otázky podľa tematických okruhov

### 1) Základy kryptografie

- [[Q01]] — Formálna definícia kryptosystému, symetrické vs. asymetrické šifry
- [[Q02]] — Architektúra bezpečnosti v RM OSI (ISO 7498-2)
- [[Q03]] — Služby a mechanizmy bezpečnosti
- [[Q04]] — Kroky pre zaistenie bezpečnej komunikácie
- [[Q05]] — Modely hrozieb: Destruction, Corruption, Removal, Disclosure, Interruption

### 2) Hašovacie funkcie a podpisy založené na hašoch

- [[Q06]] — Hašovacie funkcie: definícia, vlastnosti, bezpečnosť
- [[Q07]] — Iteračné hašovacie funkcie (Merkle–Damgård)
- [[Q08]] — Hubová konštrukcia (SHA-3 / Keccak)
- [[Q09]] — Lamportov jednorazový podpis (OTS)
- [[Q10]] — Winternitzov podpis (WOTS)

### 3) Generátory náhodných čísel

- [[Q11]] — Entropia a bezpečnosť RNG
- [[Q12]] — Požiadavky na CSPRNG
- [[Q13]] — Príklady realizácie CSPRNG

### 4) Kvantová kryptografia

- [[Q14]] — Hrozba kvantových počítačov (Shor, Grover)
- [[Q15]] — Kvantová distribúcia kľúčov (QKD): BB84, EPR, COW

### 5) Digitálne podpisy, časové razítka a eIDAS

- [[Q16]] — Digitálny podpis: definícia, požiadavky, súčinnosť s hašom
- [[Q17]] — Časové razítko (RFC 3161, TSA)
- [[Q18]] — eIDAS: elektronický podpis, pečať, časové razítko
- [[Q42]] — Vzťah digitálneho podpisu k eIDAS, úrovne podpisov

### 6) Asymetrické systémy a útoky

- [[Q19]] — McEliece (úvod; podrobne pozri [[Q40]])
- [[Q20]] — ECDH nad Fp ⚠️ *na skúške zvyčajne preskakované*
- [[Q21]] — Hastadov útok na RSA s malým exponentom
- [[Q22]] — Slepý podpis (Blind Signature) na základe RSA
- [[Q23]] — Problém diskrétneho logaritmu (DLP)
- [[Q24]] — Problém faktorizácie a útok na RSA
- [[Q31]] — Rabinov kryptosystém
- [[Q32]] — Schnorrov identifikačný a podpisový protokol
- [[Q33]] — Slabiny raw RSA
- [[Q34]] — RSA-OAEP vs. RSA-PSS

### 7) Autentizácia a protokoly

- [[Q25]] — Faktory overenia identity, kritériá výberu metódy
- [[Q26]] — Autentizačné protokoly a útoky ⚠️ *zvyčajne preskakované*

### 8) BAN logika

- [[Q27]] — BAN logika: účel, typ logiky ⚠️ *zvyčajne preskakovaná*
- [[Q28]] — Otázky a objekty BAN logiky
- [[Q29]] — Konštrukcie a pravidlá BAN logiky
- [[Q30]] — Kroky analýzy protokolov pomocou BAN

### 9) Postkvantová kryptografia (PQC)

- [[Q35]] — EdDSA vs. ECDSA ⚠️ *zvyčajne preskakované*
- [[Q36]] — EUF-CMA, SUF-CMA a tvárnosť podpisov
- [[Q37]] — Rodiny postkvantových konštrukcií
- [[Q38]] — LWE: princíp a Regevovo šifrovanie
- [[Q39]] — LWE vs. Ring-LWE vs. Module-LWE
- [[Q40]] — McEliece: generovanie kľúčov, šifrovanie, dešifrovanie
- [[Q41]] — Niederreiterov kryptosystém

### 10) Ideové návrhy

- [[Q43]] — Ideové návrhy kryptosystémov pre špecifické aplikácie

---

## 🧭 Skúškové info (rýchla pripomienka)

> [!summary] Formát skúšky
> - **5 otázok** za **60 minút**
> - **60 bodov** celkovo
> - **Vždy minimálne 1× Ideový návrh** (pozri [[Q43]])
> - Zvyčajne preskakované: Q20, Q26, Q27, Q35 (sú v poznámkach kvôli kontextu)

---

## 🧩 Concept index (atomické pojmy)

Algoritmy a primitíva:
[[concepts/AES]] · [[concepts/RSA]] · [[concepts/DES]] · [[concepts/SHA-2]] · [[concepts/SHA-3]] · [[concepts/HMAC]] · [[concepts/MAC]] · [[concepts/AEAD]] · [[concepts/ChaCha20]] · [[concepts/ECDH]] · [[concepts/ECDSA]] · [[concepts/EdDSA]] · [[concepts/Diffie-Hellman]] · [[concepts/ElGamal]] · [[concepts/Schnorr]] · [[concepts/Rabin]] · [[concepts/McEliece]] · [[concepts/Niederreiter]] · [[concepts/LWE]] · [[concepts/Kyber]] · [[concepts/Dilithium]] · [[concepts/SPHINCS+]]

Matematické pojmy:
[[concepts/Goppa-kod]] · [[concepts/DLP]] · [[concepts/Faktorizacia]] · [[concepts/CRT]] · [[concepts/Eulerova-funkcia]] · [[concepts/Eulerov-zovsobnenie]] · [[concepts/Eliptické-krivky]] · [[concepts/Mriežková-kryptografia]]

Konštrukcie a útoky:
[[concepts/Merkle-Damgard]] · [[concepts/Sponge-construction]] · [[concepts/OAEP]] · [[concepts/PSS]] · [[concepts/Birthday-attack]] · [[concepts/Length-extension-attack]] · [[concepts/Replay-attack]] · [[concepts/MitM]] · [[concepts/Side-channel]]

Štandardy a normy:
[[concepts/eIDAS]] · [[concepts/PKI]] · [[concepts/TLS]] · [[concepts/IPsec]] · [[concepts/X.509]] · [[concepts/FIPS-140]] · [[concepts/NIST-SP-800-90A]] · [[concepts/RFC-3161]]

Kvantová kryptografia:
[[concepts/QKD]] · [[concepts/BB84]] · [[concepts/Shorov-algoritmus]] · [[concepts/Groverov-algoritmus]] · [[concepts/No-cloning-teorem]]

Autentizácia:
[[concepts/BAN-logika]] · [[concepts/Nonce]] · [[concepts/MFA]] · [[concepts/PFS]] · [[concepts/Zero-Knowledge]]

---

## 🔤 Hlavné skratky (rýchly slovník)

| Skratka | Čo znamená | Stránka |
|---|---|---|
| **AES** | Advanced Encryption Standard | [[concepts/AES]] |
| **RSA** | Rivest–Shamir–Adleman | [[concepts/RSA]] |
| **ECC** | Elliptic Curve Cryptography | [[concepts/Eliptické-krivky]] |
| **ECDH** | Elliptic Curve Diffie–Hellman | [[Q20]] |
| **ECDSA** | EC Digital Signature Algorithm | [[concepts/ECDSA]] |
| **EdDSA** | Edwards-curve DSA | [[Q35]] |
| **HMAC** | Hash-based MAC | [[concepts/HMAC]] |
| **MAC** | Message Authentication Code | [[concepts/MAC]] |
| **AEAD** | Authenticated Encryption with Associated Data | [[concepts/AEAD]] |
| **XOF** | Extendable-Output Function (napr. SHAKE) | [[Q08]] |
| **OTS** | One-Time Signature | [[Q09]] |
| **WOTS** | Winternitz OTS | [[Q10]] |
| **(CS)PRNG** | (Cryptographically Secure) Pseudo-RNG | [[Q12]] |
| **TRNG** | True RNG (hardvérový zdroj entropie) | [[Q13]] |
| **DRBG** | Deterministic Random Bit Generator | [[Q13]] |
| **QKD** | Quantum Key Distribution | [[Q15]] |
| **BB84** | Bennett–Brassard 1984 protokol | [[Q15]] |
| **TSA** | Time Stamping Authority | [[Q17]] |
| **eIDAS** | EU nariadenie 910/2014 | [[Q18]] · [[Q42]] |
| **QES / AdES / SES** | Qualified / Advanced / Simple Electronic Signature | [[Q18]] · [[Q42]] |
| **DLP** | Discrete Logarithm Problem | [[Q23]] |
| **CRT** | Chinese Remainder Theorem (Čínska veta o zvyškoch) | [[Q21]] · [[Q31]] |
| **CCA / CCA2** | Chosen-Ciphertext Attack (level 2 = adaptívny) | [[Q34]] |
| **CMA** | Chosen-Message Attack | [[Q36]] |
| **EUF / SUF** | Existential / Strong Unforgeability | [[Q36]] |
| **OAEP** | Optimal Asymmetric Encryption Padding | [[Q34]] |
| **PSS** | Probabilistic Signature Scheme | [[Q34]] |
| **MFA** | Multi-Factor Authentication | [[Q25]] |
| **PUF** | Physical Unclonable Function | [[Q25]] |
| **MitM** | Man-in-the-Middle attack | [[Q26]] |
| **PQC** | Post-Quantum Cryptography | [[Q37]] |
| **LWE** | Learning With Errors | [[Q38]] · [[Q39]] |
| **NTT** | Number Theoretic Transform | [[Q39]] |
| **PFS** | Perfect Forward Secrecy | [[Q43]] |
| **HSM / QSCD** | Hardware Security Module / Qualified Signature Creation Device | [[Q17]] · [[Q18]] |
| **EUDI Wallet** | European Digital Identity Wallet (eIDAS 2.0) | [[Q42]] |

---

## ⚙️ Technické tipy pre Obsidian

> [!tip] Užitočné pluginy
> - **Spaced Repetition** – flashcards `Q::` / `A::` v poznámkach
> - **Mermaid** (core) – diagramy v `mermaid` code blokoch
> - **Callout** (core) – `> [!summary]`, `> [!tip]`, `> [!warning]`, `> [!example]`
> - **Graph view** – vizualizácia prepojení medzi otázkami a pojmami

> [!warning] LaTeX / matematika
> Vzorce sú v `$...$` (inline) alebo `$$...$$` (block). Pri exporte z Wordu sa niektoré vzorce stratili – sú prepísané do textovej / LaTeX podoby manuálne.
