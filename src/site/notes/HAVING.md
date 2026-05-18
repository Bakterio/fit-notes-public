---
{"dg-publish":true,"permalink":"/having/","tags":["#databaze/sql","#card"],"dg-note-properties":{"is-in-anki?":true,"cards-deck":"DBS","tags":["#databaze/sql","#card"]}}
---


# HAVING
#card 
filtr výsledků [[GROUP BY\|GROUP BY]] v závislosti na hodnotu [[Agregační funkce\|Agregační funkce]]
**Např.:** Seřaď země podle jejich jména, ale pouze ty, které mají více než 5 zákazníků.
```sql
SELECT Country, COUNT(CustomerID) AS [Number of Customers]
FROM Customers
GROUP BY Country
HAVING COUNT(CustomerID) > 5
```{ #1777369309343}


---
## Anki

##### Front
