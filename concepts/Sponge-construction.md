---
tags: [kry, concept, topic/has]
---
# Hubová konštrukcia (Sponge Construction)

**Sponge construction** (hubová konštrukcia) je spôsob stavby hašovacích a XOF funkcií. Využíva ju SHA-3/Keccak.

**Stav:** Fixný interný stav bitov rozdelený na dve časti:
- **Bitová šírka (rate $r$)** — „absorbuje" vstupné bloky
- **Kapacita ($c$)** — skrytá časť stavu; $c = 2 \times \text{bezpečnosť}$

**Dve fázy:**
1. **Absorpcia (*Absorbing*):** Vstupné bloky sa XOR-ujú do rate časti a aplikuje sa permutácia $f$.
2. **Vytláčanie (*Squeezing*):** Z rate časti sa extrahujú výstupné bloky (opakovane, kým nie je dosť výstupu).

**XOF (Extendable-Output Function):** Sponge prirodzene generuje výstup ľubovoľnej dĺžky — napr. SHAKE128, SHAKE256.

**Výhoda oproti Merkle-Damgård:** Imunita voči *length extension attack* (kapacita $c$ je nikdy nevystupuje).

---
## Spätné prepojenia
Detailne: [[Q08]]
Súvisí s: [[concepts/SHA-3]], [[concepts/Merkle-Damgard]]
