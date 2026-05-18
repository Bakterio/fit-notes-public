---
{"dg-publish":true,"permalink":"/primarni-klic/","tags":["#card"],"dg-note-properties":{"is-in-anki?":true,"cards-deck":"DBS","tags":["#card"],"aliases":["Primary key"]}}
---


# Primární klíč
#card 
*minimální* množina [[Atribut\|atributů]] [[Entita\|entity]], který jednoznačně [[Funkční závislost\|funkčně]] určí celou [[Relace\|relaci]]
jedna relace může mít více klíčů
neexistuje podmnožina klíče, která by také mohla být klíč{ #1772836560805}


## Postup hledání klíče relace
#card 
1) **vypsat atributy**, které *nejsou na ničem funkčně závislé* (nejsou v levé straně žádné funkční závislosti) => musí být v klíči
2) udělat **tranzitivní uzávěry levý stran všech FZ**, pokud po přidání atributů z kroku 1) mám pokrytou celou relaci, *našel jsem klíč*
3) u každého nalezeného klíče musím prokázat, že **žádná jeho podmnožina nemůže být taky klíčem** (=> musí se vyplnit *tranzitivní uzávěry všech podmnožin* všech nalezených klíčů){ #1779049258612}


---
## Anki

##### Jak by se měl pojmenovat *id* [[Entita\|entity]]?
#card 
`id_entita`
nemělo by se jmenovat pouze `id`, pak by se to mohlo plést v [[Relační algebra\|RA]]{ #1773141476932}

