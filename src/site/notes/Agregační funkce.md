---
{"dg-publish":true,"permalink":"/agregacni-funkce/","tags":["#databaze/sql","#card"],"dg-note-properties":{"is-in-anki?":true,"cards-deck":"DBS","tags":["#databaze/sql","#card"]}}
---


# Agregační funkce
#card 
**množina dat $\to$ jedno číslo**
(funkce bere *množinu dat* (výsledek dotazu [[SELECT\|SELECT]]) a *vrací jedno číslo*)
**Např.:** MIN, MAX, COUNT, SUM, AVG
###### Použití agregační funkce:
```sql
SELECT COUNT(*)
FROM zamestnanici
WHERE plat < 10000
```{ #1777366429909}


## (Ne)ignorování NULL hodnot
#card 
`count(*)` započítává i NULL hodnoty
`count(A)` nezapočítává NULL hodnoty{ #1777366429914}


---
## Anki

##### Front
