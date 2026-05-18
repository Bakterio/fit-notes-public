---
{"dg-publish":true,"permalink":"/view/","tags":["#databaze/sql","#card"],"dg-note-properties":{"is-in-anki?":false,"cards-deck":"DBS","tags":["#databaze/sql","#card"]}}
---


# VIEW
#card 
*= POHLED, virtuální relace*
chová se to jako samostatná tabulka, ale je to *makro*, pod kterým je select
**Např.:** Z databáze studentů si mohu udělat view pražáci, kde budu mít pouze lidi, kteří bydlí v Praze
###### Užití
**Ochrana dat**
Pokud některý uživatel nemá vidět nějaký atributy (plat), nedám mu přístup k tabulce databázi, ale jenom view nad touto tabulkou, kde plat nebude.
**Zjednodušení komplexity.**
Složité relace v tabulce mohu pro další zpracování prezentovat jako jednu tabulku.{ #1777374237133}


## Update dat v pohledu
#card 
data se **změní v původních tabulkách**, pokud v pohledu nepoužívají např. [[Agregační funkce\|Agregační funkce]]
(pokud se nejedná o [[VIEW#Materialized view\|#Materialized view]]){ #1778266787865}


## DROP VIEW
#card 
*vymaže* se VIEW
*nevymažou* se data (původní tabulky){ #1777374237158}


## Check option
#card 
Upozorní mě, když změna hodnoty argumentu vyhodí záznam z VIEW.
**Např.:** Tabulka Pražáci.
Pokud bych měl view Pražáci a chtěl studenta přestěhovat do Plzně, vypadl by my pak z view Pražáci. Check option toto zamezí.{ #1777375061892}


## Materialized view
#card 
tabulka *není virtuální*, ale opravdu se *vytvoří* a data se do ní zkopírují
když změním data v materialized view, *nepropíšou se do původních tabulek* (jsou uložené odděleně)
dá se pomocí nich udělat **cache**{ #1777375061902}


---
## Anki

##### Front
