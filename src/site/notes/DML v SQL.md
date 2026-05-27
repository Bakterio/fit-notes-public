---
{"dg-publish":true,"permalink":"/dml-v-sql/","tags":["databaze/sql"],"dg-note-properties":{"is-in-anki?":true,"cards-deck":"DBS","tags":["databaze/sql"]}}
---


# DML v [[SQL\|SQL]]
#card 
*= data manipulation language*
příkazy INSERT, UPDATE, DELETE, MERGE
zpracování transakcí
při zpracování DML se berou v potaz [[Integritní omezení\|Integritní omezení]]{ #1777373892208}


## DELETE
#card 
smaže záznamy z tabulky podle filtru
Smazat film se jménem „Vrchní prchni“
```sql
DELETE FROM Filmy
WHERE jmeno_f = "Vrchni prchni"
```{ #1777373892362}


## UPDATE
#card 
změní hodnotu atributu
```sql
UPDATE Zakaznici
SET jmeno = "Novak"
WHERE rod_c = "123456"
```
může se naspat jako poddotaz při nastavování výchozí hodnoty nového sloupce pomocí ALTER TABLE{ #1777373892372}


## INSERT
#card 
vloží nový řádek do tabulky
nejprve vypsat, jaké atributy a v jakém pořadí vkládám a potom data
```sql
INSERT INTO Zakaznici (rod_c, jmeno) VALUES ('123456', 'Novak')
```
mohu volat insert spolu s podmínkou
do tabulky dám nějaká data z jiných tabulek, která splňují nějakou podmínku{ #1777373892380}


---
## Anki

##### Front
