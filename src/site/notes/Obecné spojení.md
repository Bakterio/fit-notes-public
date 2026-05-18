---
{"dg-publish":true,"permalink":"/obecne-spojeni/","tags":["#dbs/relacni-algebra","#card"],"dg-note-properties":{"is-in-anki?":true,"cards-deck":"DBS","tags":["#dbs/relacni-algebra","#card"]}}
---


# Obecné spojení
#card 
spojení podle ručně zadané podmínky
`zvire [zvire.id_kmotr = osetrovatel.id_osetrovatel] osetrovatel`
vznikne tak relace, ve které jsou všechny atributy obou dvou entit
###### Rozdíl oproti natural join
Data, podle kterých se spojovalo budou ve výsledku dvakrát. 
(`id_kmotr` a `id_osetrovatel` jsou duplikáty)
![ra-obecne-spojeni.png](/img/user/source/ra-obecne-spojeni.png){ #1773749994165}


## Výběr atributů pomocí závorek `<>`
#card 
`zvire [zvire.id_kmotr = osetrovatel.id_osetrovatel> osetrovatel`
ve výsledku budou *pouze atributy ošetřovatele*, protože na něj ukazuje šipka
![ra-obecne-spojeni-filtr.png](/img/user/source/ra-obecne-spojeni-filtr.png){ #1773749994171}


---
## Anki

##### Front
