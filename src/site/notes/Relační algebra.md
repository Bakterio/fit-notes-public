---
{"dg-publish":true,"permalink":"/relacni-algebra/","tags":["#dbs/relacni-algebra","#card"],"dg-note-properties":{"is-in-anki?":false,"cards-deck":"DBS","tags":["#dbs/relacni-algebra","#card"],"aliases":["RA"]}}
---


# Relační algebra
#card 
**pracuje s daty a jejich vztahy** => vzor pro příkaz [[SELECT\|SELECT]] v [[SQL\|SQL]]
každý výraz v RA se *dá převést na [[SELECT\|SELECT]] v [[SQL\|SQL]]*
neumí tedy vytvářet data, umí se pouze dotazovat
vrací *množinu záznamů*
jeden řádek v tabulce je [[n-tice\|n-tice]]{ #1772834721859}


## Operace
#card 
Dá se s nimi vyjádřit jakákoli operace. Tvoří něco jako [[Universální systém logických spojek\|Universální systém logických spojek]]
###### Množinové operace
1. [[Kartézský součin\|Kartézský součin]] - $\times$
2. sjednocení - $\cup$
3. průnik - $\cap$
4. množinový rozdíl $\setminus$
5. [[Relační dělení\|Relační dělení]]
###### Filtrování řádků a sloupců
6. [[Selekce\|Selekce]] - `()`
7. [[Projekce\|Projekce]] - `[]`
###### Přejmenování
- nemění skutečnou hodnotu
8. přejmenování [[Relace\|Relace]] $\to$
9. přejmenování atributu [[Relace\|Relace]]
###### Spojování
10. [[Spojení\|Spojení]] - `* []` ([[Přirozené spojení\|Přirozené spojení]], [[Obecné spojení\|Obecné spojení]])
11. [[Polospojení\|Polospojení]] - `<* *>` nebo `<] [>` ([[Levé spojení\|Levé spojení]], [[Pravé spojení\|Pravé spojení]], [[Vnější spojení\|Vnější spojení]])
12. [[Antijoin\|Antijoin]] - `<* *>` nebo `<] [>` (nad znaky je negace){ #1772834721866}


## Priorita operátorů
#card 
1) unární operátory
2) závorkování pomocí `{}`{ #1772835557229}


---
## Anki

##### Jaký objekt vrací operace v [[Relační algebra\|relační algebře]]?
#card 
je to „zobrazení“ $\text{relace} \to \text{relace}$
operace se dají skládat za sebe, podobně jako [[Shell#Kolona příkazů\|roura v shell]]{ #1772835433260}


##### Jak donutit [[SQL\|SQL]], aby se chovalo *množinově* jako [[Relační algebra\|Relační algebra]]?
#card 
za všechno dát slovo `DISTINCT`, smaže duplikáty
(v množině nejsou duplikáty povoleny){ #1774808301159}

