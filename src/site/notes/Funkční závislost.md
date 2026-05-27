---
{"dg-publish":true,"permalink":"/funkcni-zavislost/","dg-note-properties":{"is-in-anki?":true,"cards-deck":"DBS","tags":null}}
---


# Funkční závislost
#card 
množina atributů $M$ jednoznačně určuje jinou množinu atributů $N$
pro *každou* $M$ *existuje nejvýše jedna* $N$
jedno z [[Integritní omezení\|integritních omezení]]
*rodné číslo => pohlaví, vek*
*rodné číslo* funkčně určuje *pohlaví* a *věk*
*pohlaví* a *věk* jsou funkčně závislé na *rodném čísle*{ #1779042798740}


vlastnostem funkčních závislostí se říká *Armstrongova pravidla*

## Triviální funkční závislost
#card 
**množina atributů vždy funkčně definuje jakoukoli svou podmnožinu**
Vždy platí:
$PS \to PS$
$PS \to P$
$PS \to S${ #1779043506965}


## Tranzitivita
#card 
pokud:
*rodné číslo -> příjmení* a *příjmení -> studijní referentka*
pak:
*rodné číslo -> studijní referentka*{ #1779043785565}


## Kompozice pravé/levé strany
#card 
pokud:
*rodné číslo -> příjmení* a *rodné číslo -> místo narození*
pak:
*rodné číslo -> příjmení, místo narození*{ #1779043916611}


## Dekompozice pravé/levé strany
#card 
pokud:
*rodné číslo -> příjmení, místo narození*
pak:
*rodné číslo -> příjmení* a *rodné číslo -> místo narození*{ #1779043916619}


## Tranzitivní uzávěr atributů X
#card 
*značení:* $X^+$
množina všech atributů funkčně závislých na X
*neboli:* Pokud znám $X$, co všechno znám?{ #1779048327293}


## Kanonické pokrytí
#card 
zjednodušení množiny funkčních závislostí tak, že pouze jeden atribut určuje druhý
*Z:*
$A \to B,C$
*Do:*
$A \to B$
$A \to C$
Pokud se při dekompozici zjistí, že je nějaká FZ redundantní, odstraní se.{ #1779218239849}


---
## Anki

##### Front
