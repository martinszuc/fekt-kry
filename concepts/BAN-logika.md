---
tags: [kry, concept, topic/banlogika]
---
# BAN logika (Burrows–Abadi–Needham)

**BAN logika** je formálna metóda na analýzu a verifikáciu **autentizačných protokolov**, navrhnutá Burrowsom, Abadiom a Needhamom (1989).

**Typ:** Epistemická modálna logika — modeluje *vieru* (*belief*) účastníkov, nie absolútnu pravdu.

**Základné konštrukcie:**
- $P \mid\!\equiv X$ — $P$ *verí* $X$
- $P \triangleleft X$ — $P$ *vidí* $X$ (prijal správu)
- $\#(X)$ — $X$ je *čerstvé* (nonce)
- $P \mid\!\sim X$ — $P$ *niekedy vyslovil* $X$

**3 inferenčné pravidlá:** Message Meaning, Nonce Verification, Jurisdiction.

**5 krokov analýzy:** Idealizácia → Predpoklady → Ciele → Odvodzovanie → Vyhodnotenie.

**Historický dopad:** BAN odhalila chyby v Needham-Schroeder protokole (1978) — opravené ako Needham-Schroeder-Lowe (1995).

---
## Spätné prepojenia
Detailne: [[Q27]], [[Q28]], [[Q29]], [[Q30]]
Súvisí s: [[concepts/Nonce]], [[concepts/Replay-attack]]
