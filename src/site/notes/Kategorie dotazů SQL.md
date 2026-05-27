---
{"dg-publish":true,"permalink":"/kategorie-dotazu-sql/","tags":["databaze/sql"],"dg-note-properties":{"is-in-anki?":true,"cards-deck":"DBS","tags":["databaze/sql"]}}
---


# Kategorie dotazů [[SQL\|SQL]]

## Dotaz kategorie D
#card 
**jeden člen entity A má vztah ke všem členům entity B**
*Př.:* ID_ZAKAZNIKU, kteří si zarezervovali každou zelenou loď
###### Řešení v [[Relační algebra\|RA]]
udělat si universum pomocí kartézského součinu
odečíst od něj ty, které neplatí => získám ty, které platí
```sql
rezervace[id_zak,id_lod] ÷ {lod(barva='zelena')[id_lod]}
```{ #1774812632302}


## Dotaz kategorie C
#card 
vztah výhradně v něčemu
*Př.:* Zákazníci, kteří si rezervovali pouze lodě typu t2.
###### Řešení v [[Relační algebra\|RA]]
**toto je důležité:**
rezervovali-si-pouze-typu-t2 := rezervovali-si-nějakou-typu-t2 - rezervovali-si-nejakou-jinou-nez-typu-t2
```sql
rezervovali-si-nejakou-typu-t2 := {rez*lod}(typ='t2')[id_zak]
rezervovali-si-nejakou-jinou-nez-t2 := {rez*lod}(typ!='t2')[id_zak]
rezervovali-si-pouze-typu-t2 := rezervovali-si-nějakou-typu-t2 - rezervovali-si-nejakou-jinou-nez-typu-t2
```{ #1774812632307}


---
## Anki

##### Front
