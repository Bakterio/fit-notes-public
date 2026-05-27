---
{"dg-publish":true,"permalink":"/kvantifikatory-v-sql/","tags":["databaze/sql"],"dg-note-properties":{"is-in-anki?":true,"cards-deck":"DBS","tags":["databaze/sql"]}}
---


# Kvantifikátory v SQL
umí [[Existenční kvantifikátor\|Existenční kvantifikátor]] i [[Obecný kvantifikátor\|Obecný kvantifikátor]]

## EXISTS
#card 
používá se s [[WHERE\|WHERE]]
implementuje [[Existenční kvantifikátor\|Existenční kvantifikátor]]
vrátí *true*, pokud [[Poddotaz\|Poddotaz]] *něco vrátí*
vrátí *false*, pokud [[Poddotaz\|Poddotaz]] *nic nevrátí*
**Např.:** Dodavatelé, kteří dodávají produkt levnější než 10$.
```sql
SELECT SupplierName
FROM Suppliers
WHERE EXISTS (
  SELECT ProductName
  FROM Products
  WHERE Products.SupplierID = Suppliers.supplierID AND Price < 10
); 
```{ #1777370999042}


## [[Obecný kvantifikátor\|Obecný kvantifikátor]]
#card 
není v [[SQL\|SQL]] přímo implementováváno
dělá se pomocí **negace EXISTS** + **negace výroku**
**Např.:** Kino, které hraje *všechna* představení.
```sql
SELECT nazev
FROM kina K
WHERE NOT EXISTS (SELECT 1
	FROM predstaveni P
	WHERE K.id_kina <> P.id_kina);
```{ #1777372178310}


---
## Anki

##### Front
