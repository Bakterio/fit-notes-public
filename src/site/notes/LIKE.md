---
{"dg-publish":true,"permalink":"/like/","tags":["#databaze/sql","#card"],"dg-note-properties":{"is-in-anki?":true,"cards-deck":"DBS","tags":["#databaze/sql","#card"]}}
---


# LIKE
#card 
kontroluje, jestli výraz odpovídá některému řetězci
`%` - skupina znaků (i prázdná), jako `*` v [[grep\|grep]]
`_` - právě jeden výraz, jako `?` v [[grep\|grep]]
k excapovaní znaků se použije `\`
**Např.:** Všichni zákazníci, kteří začínají na „a“.
```spl
SELECT * FROM Customers
WHERE CustomerName LIKE 'a%'; 
```{ #1777370854406}


---
## Anki

##### Front
