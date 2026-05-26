---
tags: [kry, concept, topic/utoky]
---
# Replay Attack (Útok zopakovaním)

**Replay attack** je útok, pri ktorom útočník **zachytí platné autentizačné správy** z predchádzajúcej relácie a **znovu ich pošle** verifikátoru neskôr, aby sa vydával za legitímneho účastníka.

**Príklad:**
```
1. Alice → Bob: {heslo, timestamp=09:00}  [útočník zachytí]
2. O hodinu neskôr útočník → Bob: {heslo, timestamp=09:00}
3. Bob bez ochrany akceptuje → útočník je "Alice"
```

**Ochrana:**
- **Nonce** (*Number used ONCE*) — každá relácia má unikátne náhodné číslo; správa ho musí obsahovať
- **Časové razítka** — správa platí len v časovom okne (napr. ±5 minút)
- **Sekvenčné čísla** — každá správa má rastúce číslo; staré odmietané

**Súvislosť:** BAN logika formálne overuje, či protokol odoláva replay útoku ([[Q28]], [[Q29]]).

---
## Spätné prepojenia
Kontext: [[Q26]], [[Q28]]
Súvisí s: [[concepts/Nonce]], [[concepts/BAN-logika]]
