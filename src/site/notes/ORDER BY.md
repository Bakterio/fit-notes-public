---
{"dg-publish":true,"permalink":"/order-by/","tags":["databaze/sql"],"dg-note-properties":{"is-in-anki?":true,"cards-deck":"DBS","tags":["databaze/sql"]}}
---


# ORDER BY
#card 
**seřadí záznamy** podle nějakého atributu
pro pořadí se používá *ASC|DESC*
```sql
SELECT * FROM Products
ORDER BY Price;
```{ #1777369531291}


---
## Anki

##### Jak seřadit záznamy *vzestupně*?
#card 
`ASC` se může vynechat
```sql
SELECT * FROM Products
ORDER BY Price ASC;
```{ #1777369531301}


##### Jak seřadit záznamy *sestupně*?
#card 
```sql
SELECT * FROM Products
ORDER BY Price DESC;
```{ #1777369531308}

