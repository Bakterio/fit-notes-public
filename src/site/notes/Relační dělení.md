---
{"dg-publish":true,"permalink":"/relacni-deleni/","tags":["#dbs/relacni-algebra","#card"],"dg-note-properties":{"is-in-anki?":true,"cards-deck":"DBS","tags":["#dbs/relacni-algebra","#card"]}}
---


# Relační dělení
#card 
`A(x,y) ÷ B(y)` nebo `A[x, y] ÷ B[y]`
*Podmínka pro dělení:* `B(y)` $\subset$ `A(y)`
vrátí všechny záznamy z `A` (selekce x), které jsou v relaci s `B`
###### Příklad: zákazníci si rezervují lodě
**Chci dostat:** Zákazníci, kteří si rezervovali všechny lodě (ne najednou).
`REZERVACE[id_zakaznik, id_lod] děleno LOD[id_lod]`
For every row in `REZERVACE`
1) vybere `id_zakaznik`
2) koukne se, jestli jeho `id_lod` obsahujou všechny `id_lod` z `LOD`
3) pokud tak platí, vrátí *id_zakaznik*, jinak nic
získám pouze množinu s `is_zakaznik`, musím ji spojit s tabulkou ZAKAZNICI, abych získal všechny jejich data{ #1774807739860}


---
## Anki

##### Jaká podmínka musí platit pro [[Relační dělení\|Relační dělení]]?
`A(x,y) ÷ B(y)`
#card 
`B(y)` $\subset$ `A(y)`{ #1774807739864}

