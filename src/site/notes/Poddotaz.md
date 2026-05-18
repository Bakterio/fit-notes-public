---
{"dg-publish":true,"permalink":"/poddotaz/","tags":["#databaze/sql","#card"],"dg-note-properties":{"is-in-anki?":true,"cards-deck":"DBS","tags":["#databaze/sql","#card"]}}
---


# Poddotaz
#card 
pokud se používá v podmínce `=` musí se porovnávat dvě hodnoty, ani jedna nesmí být množina{ #1777370382643}


## Nevztažené poddotazy
#card 
vrátí jednu hodnotu, kterou dosadím do výrazu
*nejsou navázány* na vnější dotaz => **vyhodnotí se pouze jednou**
**Např.:** Jméno a přímení zaměstnanců, kteří mají největší možný plat.
```sql
SELECT jmeno, prijmeni
FROM zamestnanici
WHERE plat = (SELECT MAX(plat)
				FROM zamestnanici)
```{ #1777370382653}


## Vztažené poddotazy
#card 
vrátí jednu hodnotu, kterou dosadím do výrazu
*jsou navázány* na vnější dotaz => **vyhodnocují se s každým záznamem** [[FROM\|FROM]]
**Např.:** Jméno a přímení zaměstnanců, kteří mají největší možný plat.{ #1777370382662}


---
## Anki

##### Front
