---
{"dg-publish":true,"permalink":"/transformace-konceptualniho-schematu-na-relacni/","tags":["databaze/sql"],"dg-note-properties":{"is-in-anki?":true,"cards-deck":"DBS","tags":["databaze/sql"]}}
---


[[Fleeting-notes/DBS.p6\|DBS.p6]]

# Transformace konceptuálního schématu na relační
#card 
![schema-pro-transformaci-nevyhovujici-pojmenovani.png](/img/user/source/schema-pro-transformaci-nevyhovujici-pojmenovani.png)
1) **Popsat entity, které jsou co nejvíce osamocené** = kde není kuří noha a je nepovinnost
2) postupovat k dalším entitám
3) nakonec popsat [[Specializace\|specializace]]{ #1774813436251}


## Transformace a značení jednoduché entity
#card 
`Lekar(lekar_id, *jmeno, *prijmeni)`
*Primární klíč se podtrhne* (ale v markdownu to nejde)
*před povinné atributy* se napíše `*` *hvězdička*{ #1774813436256}


## Transformace tabulky s cizím klíčem
#card 
specifikuji, že **cizí klíč musí zároveň existovat jako primární klíč** v oné tabulce
`Zvire(id_zvire, *jmeno, datum_narozeni, *pohlavi, id_druh)`
`zvire[id_druh]` $\subseteq$ `Druh[id_druh]`
###### Automatické mazání
pokud smažu určitý druh zvířete, automaticky se smažou i všechny zvířata tohoto druhu
jinak by byla poručena tato podmínka
(funguje jako [[Drop table#drop table cascade\|Drop table#drop table cascade]]){ #1774813737577}


## Transformace smyčky
#card 
![schema-pro-transformaci-nevyhovujici-pojmenovani.png](/img/user/source/schema-pro-transformaci-nevyhovujici-pojmenovani.png)
*prohlídka zvířete* má dvě vazby na *lekar*
musí se přejmenovat cizí klíč, aby bylo jasný jaká to je vazba
dva atributy entity se nemohou jmenovat stejně
`Prohlidka_zvirete[prohlizi]` $\subseteq$ `lekar[lekar_id]`
`Prohlidka_zvirete[pripomaha]` $\subseteq$ `lekar[lekar_id]`{ #1774813737580}


## Transformace [[ISA hiearchie\|ISA hiearchie]]
#card 
všechny atributy podtypů se dají jako **atributy jedné nadentity**
pomocí *view* mohu na nadentitu koukat jako na jednotlivé podentity
musí se zajistit, aby byly **vyplněný sloupce pouze jedný entity** a druhý ne
`Objekt(id_objekt, *adresa, objem, vybebeni, ma_internet, plocha, clenitost)`
`Objekt[id_krmic]` $\subseteq$ `Krmic[id_krmic]`
`Chek((objem IS NOT NULL and plocha IS NOT NULL) OR (objem IS NULL and plocha IS NOT NULL))`{ #1774813919977}


## Transformace M:N
#card 
![schema-pro-transformaci-nevyhovujici-pojmenovani.png](/img/user/source/schema-pro-transformaci-nevyhovujici-pojmenovani.png)
vytvoří se [[Vztahová entita\|Vztahová entita]]
`Ma_pridelen(id_zvire, id_objekt)`
`Ma_pridelen[id_zvire]` $\subseteq$ `Zvire[id_zvire]`
`Ma_pridelen[id_objekt]` $\subseteq$ `Objekt[id_objekt]`
Pokud je na slabou vztahovou entitu navázán další objekt, musí se u tohoto objektu dělat
`Platba[id_zvire, id_objekt]` $\subseteq$ `Ma_pridelen[id_zvire, id_objekt]`{ #1774813919979}


---
## Anki

##### Jak podle relačního zápis entity poznat počet spojů entity?
#card 
je stejný jako *počet cizích klíčů*{ #1774813737583}

