---
{"dg-publish":true,"permalink":"/create-table/","tags":["#databaze/sql","#card"],"dg-note-properties":{"is-in-anki?":true,"cards-deck":"DBS","tags":["#databaze/sql","#card"]}}
---


# Create table
#card 
vytvoří tabulku s danýma [[Atribut\|atributama]]
```sql
CREATE TABLE Persons (
  PersonID int PRIMARY KEY,
  LastName varchar(255) NOT NULL,
  FirstName varchar(255),
  Address varchar(255),
  City varchar(255)
);
```{ #1774809567861}


---
## Anki

##### Front
