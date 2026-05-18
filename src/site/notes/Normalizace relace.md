---
{"dg-publish":true,"permalink":"/normalizace-relace/","tags":["#dbs/normalizace","#card"],"dg-note-properties":{"is-in-anki?":false,"cards-deck":"DBS","tags":["#dbs/normalizace","#card"]}}
---


[YT video](https://youtu.be/GFQaEYEc8_8)

# Normalizace relace
#card 
rozložení dat do [[Entita\|tabulek]] za užití [[Funkční závislost\|funkčních závislostí]]
snižuje riziko [[Aktualizační anomálie\|aktualizačních anomálií]]
1) najít [[Funkční závislost\|Funkční závislost]]i mezi daty
2) zvolit klíč schématu - [[Primární klíč#Postup hledání klíče relace\|Primární klíč#Postup hledání klíče relace]]
3) otestovat na [[Třetí normální forma\|Třetí normální forma]]/[[Boyce-Coddova normální forma\|Boyce-Coddova normální forma]]
4) pokud nevyhovuje => dekomponovat relaci => rekurzivně pokračovat na bod 1){ #1779049966642}


## Normální formy
[[První normální forma\|První normální forma]]
[[Druhá normální forma\|Druhá normální forma]]
[[Třetí normální forma\|Třetí normální forma]]
[[Boyce-Coddova normální forma\|Boyce-Coddova normální forma]]

## Normalizace dekompozicí
#card 
převedení schématu do [[Třetí normální forma\|Třetí normální forma]] nebo [[Boyce-Coddova normální forma\|Boyce-Coddova normální forma]] za účelem redukce [[Aktualizační anomálie\|aktualizačních anomálií]]
platí:
1) [[Normalizace relace#Pokrytí původní množiny funkčních závislostí\|#Pokrytí původní množiny funkčních závislostí]]
2) [[Normalizace relace#Bezztrátová dekompozice\|#Bezztrátová dekompozice]]{ #1779115012584}


### Pokrytí původní množiny funkčních závislostí
#card 
[[Tranzitivní uzávěr\|Tranzitivní uzávěr]] FZ dekomponovaných relací musí být stejný jako [[Tranzitivní uzávěr\|Tranzitivní uzávěr]] FZ původní relace{ #1779115012589}


### Bezztrátová dekompozice
#card 
dekompozicí nesmí vzniknout ani zaniknout žádná data
spojením (joinem) dekomponovaných relací musí vzniknout původní relace{ #1779115012594}


---
## Anki

##### Existuje pouze jeden správný výsledek, ke kterému mohu dojít dekompozicí relace?
#card 
ne, dekompozicí mohu dojít k více výsledkům{ #1779115012597}

