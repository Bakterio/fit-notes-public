---
{"dg-publish":true,"permalink":"/in/","tags":["#databaze/sql","#card"],"dg-note-properties":{"is-in-anki?":true,"cards-deck":"DBS","tags":["#databaze/sql","#card"]}}
---


# IN
#card 
použije se s [[WHERE\|WHERE]]
zajímá mě, jestli nějaký prvek leží v množině
**Např.:** Adresy všech kin, které hrají film samotáři.
```sql
SELECT distinct adresa
FROM kina
WHERE nazev_k IN
	(SELECT nazev_k FROM predstaveni
	WHERE jmeno_f = ’Samotáři’)
```{ #1777371458191}


---
## Anki

##### Front
