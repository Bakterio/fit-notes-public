---
{"dg-publish":true,"permalink":"/obnova-databaze-po-padu/","tags":["#databaze","#card"],"dg-note-properties":{"is-in-anki?":false,"cards-deck":"DBS","tags":["#databaze","#card"]}}
---


# Obnova databáze po pádu
#card 
při zpracovávání transakce se vytváří změnové vektory, kde každý mění jeden řádek

## Změnový vektor
popisuje změnu jednoho řádku
ukládají se do úložiště WAL - write and lock

## Žurnál
umožňuje zachovat atomicitu a durability z [[ACID vlastnosti transakcí\|ACID vlastnosti transakcí]]
zapisuje změny
nahrají se z něj nedokončené transakce po pádu systému

---
## Anki

##### Front
