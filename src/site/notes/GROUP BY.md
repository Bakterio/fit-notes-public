---
{"dg-publish":true,"permalink":"/group-by/","tags":["databaze/sql"],"dg-note-properties":{"is-in-anki?":true,"cards-deck":"DBS","tags":["databaze/sql"]}}
---


# GROUP BY
#card 
*= seskupování řádků*
příkaz `GROUP BY jmeno_filmu`, kde se seřazuje podle jména filmu{ #1777369720486}


## Pořadí vyhodnocení výrazu s `GROUP BY`
#card 
```sql
SELECT obsazeni1.jmeno_f, COUNT (herec) AS pocet_hercu
FROM obsazeni1, filmy
WHERE obsazeni1.jmeno_f = filmy.nazev AND rok = 2011
GROUP BY obsazeni1.jmeno_f
HAVING COUNT(herec) >= 2
ORDER BY jmeno_f;
```
1) [[FROM\|FROM]] - zdroj dat
2) [[WHERE\|WHERE]]- první filtr dat
3) [[GROUP BY\|GROUP BY]] - seskupení dat
4) [[HAVING\|HAVING]] - selekce v závislosti na [[Agregační funkce\|Agregační funkce]]
5) [[ORDER BY\|ORDER BY]] - seřazení výsledku{ #1777369720494}


---
## Anki

##### Front
