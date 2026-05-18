---
{"dg-publish":true,"permalink":"/transformace-relacniho-schematu-na-databazi/","tags":["#dbs/relacni-algebra","#databaze/sql","#card"],"dg-note-properties":{"is-in-anki?":true,"cards-deck":"DBS","tags":["#dbs/relacni-algebra","#databaze/sql","#card"]}}
---


# Transformace relačního schématu na databázi

## 1:1

### Povinná, povinná
#card 
![k11pp.png](/img/user/source/k11pp.png)
=> něco je špatně
**vytvoří se pouze jedna tabulka**
pomocí view mohu upravovat, jestli se na tabulku koukám jako na zaměstnance nebo auto{ #1774811658502}


### Povinná, nepovinná
#card 
![k11pn.png](/img/user/source/k11pn.png)
vůz bude mít v sobě uložený cizí klíč auta, který *bude* povinný atribut
vztah je tedy nesymetrický
v tabulce zaměstnanec není žádný „odkaz“ na vůz{ #1774811658507}


### Nepovinná, nepovinná
#card 
![k11nn.png](/img/user/source/k11nn.png)
vůz bude mít v sobě uložený cizí klíč auta, který *nebude* povinný atribut
vztah je tedy nesymetrický
v tabulce zaměstnanec není žádný „odkaz“ na vůz{ #1774811658510}


## 1:N

### Povinná účast u determinantu
#card 
![k1povinna-k-determinaktu.png](/img/user/source/k1povinna-k-determinaktu.png)
kde je kuří noha, tam bude cizí klíč
*Př.:* klíč bude uložen v tabulce `PACIENT` a bude **povinný**
vztah je asimetrický{ #1774811658514}


### Nepovinná účast u determinantu
#card 
![k1nepovinna-k-determinaktu.png](/img/user/source/k1nepovinna-k-determinaktu.png)
kde je kuří noha, tam bude cizí klíč
*Př.:* klíč bude uložen v tabulce `PACIENT` a bude **nepovinný**
vztah je asimetrický{ #1774811658519}


### Rekurzivní vztah
viz [[Rekurzivní vztah entit\|Rekurzivní vztah entit]]

## M:N

### [[Vztahová entita\|Vztahová entita]] je silná
#card 
![kmn-silna.png](/img/user/source/kmn-silna.png)
vytvoří se (mezitabulka) [[Vztahová entita\|Vztahová entita]], ta má dva sloupce
každý obsahuje cizí klíč k jedné z tabulek
silná => *bude* mít svoje id => bude mít primary-key{ #1774811658523}


### [[Vztahová entita\|Vztahová entita]] je slabá
#card 
![kmn-slaba.png](/img/user/source/kmn-slaba.png)
vytvoří se (mezitabulka) [[Vztahová entita\|Vztahová entita]], ta má dva sloupce
**každý ze dvou sloupců obsahuje cizí klíč k jedné z tabulek**
slabá => vztahová tabulka *nebude* mít svoje id => *nemá* [[Primární klíč\|Primární klíč]]
identifikuje se pomocí Kina a Filmu{ #1774811658528}


### Specializace a [[Specializace\|Specializace]]
#card 
specializace budou mít jako cizí klíč hlavní entitu{ #1774811658532}


---
## Anki

##### Front
