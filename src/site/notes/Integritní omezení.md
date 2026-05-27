---
{"dg-publish":true,"permalink":"/integritni-omezeni/","dg-note-properties":{"is-in-anki?":true,"cards-deck":"DBS","tags":null}}
---


# Integritní omezení
#card 
omezujeme, která data se mohou vyskytovat v [[Relace\|relaci]]
ty, které nejdou zformulovat pomocí [[Relační algebra\|RA]] se píšou do poznámky
čísluje se se jako `IOn`, kde $n \in \mathbb N$
dají se *pojmenovat*, hodí se pro debugging
#### Příklady integritních omezení
**primární klíče** - musí splňovat podmínky pro primární klíče
**cizí klíče** - pro cizí klíč musí existovat záznam, kde číslo figuruje jako primární klíč 
**slovní omezení**: 
- „Jeden film se nehraje ve více než třech kinech“ 
- nedá se zformulovat v relační algebře{ #1772837162804}


## Způsoby kontroly integritních omezení
#card 
**DEFFERED**
IO se kontrolují až na konci [[Transakce\|Transakce]]
= kontrolují se těsně před příkazem commit
**IMEDIATE**
IO se kontrolují po každém jednotlivém příkazu{ #1777375405418}


---
## Anki

##### Front
