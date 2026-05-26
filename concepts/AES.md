---
tags: [kry, concept, topic/symetria]
---
# AES — Advanced Encryption Standard

**AES** (*Advanced Encryption Standard*) je symetrická bloková šifra štandardizovaná NIST-om v roku 2001 (FIPS 197). Pôvodný algoritmus sa volá **Rijndael** (autori: Daemen a Rijmen).

**Parametre:**
- Veľkosť bloku: pevne **128 bitov**
- Dĺžka kľúča: **128 / 192 / 256 bitov**
- Počet kôl: 10 / 12 / 14 (podľa dĺžky kľúča)

**Princíp:** Substitučno-permutačná sieť (SPN) — každé kolo pozostáva z krokov SubBytes, ShiftRows, MixColumns, AddRoundKey.

**Módy prevádzky:** ECB (nebezpečný), CBC, CTR, GCM (AEAD), CCM.

**Použitie:** TLS, Wi-Fi (WPA2/3), šifrované disky, VPN, SRTP.

---
## Spätné prepojenia
Používa sa v: [[Q01]], [[Q04]], [[Q13]], [[Q37]], [[Q43]]
Súvisí s: [[concepts/AEAD]], [[concepts/ChaCha20]], [[concepts/DES]]
