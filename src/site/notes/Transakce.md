---
{"dg-publish":true,"permalink":"/transakce/","tags":["#databaze","#card"],"dg-note-properties":{"is-in-anki?":true,"cards-deck":"DBS","tags":["#databaze","#card"]}}
---


# Transakce
#card 
zajišťuje konzistenci databáze
více změn nad databází se provede najednou
na začátku a na konci transakce musí být [[Databáze\|Databáze]] v [[Konzistentní stav\|konzistentním stavu]]{ #1777373630269}


## COMMIT
#card 
příkaz [[SQL\|SQL]]
zkusí provést transakci{ #1777373630279}


## ROLLBACK
#card 
příkaz [[SQL\|SQL]]
vrátí transakci
vymaže všechny změny, které transakce udělala{ #1777373630287}


## Safepoint
#card 
když si myslím, že nějaká operace nemusí vždy provést
pokud operace selže, pak se nevrací celá transakce, ale vrací se pouze k poslednímu safepointu{ #1777373630294}


### Autocommit
#card 
**on** - vždy po zadání příkazu se příkaz hned provede
**off** - zadané příkazy se provednou najednou až po příkazu COMMIT{ #1777373630301}


## Stavy transakce
#card 
![dbs-stavy-transakce.png](/img/user/source/dbs-stavy-transakce.png)
- **A**ctive - zpracovávání transakce
- **P**artially **C**ommitted - po provedení poslední operace transakce
- **C**ommitted - po úspěšném zakončení, po potvrzení operace COMMIT
- **F**ailed - nastala chyba, nelze pokračovat v transakci
- **AB**orted - po skončení ROLLBACK, databáze se uvede do stavu před začátkem transakce{ #1779124713496}


---
## Anki

##### Front
