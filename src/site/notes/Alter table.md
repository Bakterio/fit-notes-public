---
{"dg-publish":true,"permalink":"/alter-table/","tags":["databaze/sql"],"dg-note-properties":{"is-in-anki?":true,"cards-deck":"DBS","tags":["databaze/sql"]}}
---


# Alter table
#card 
upraví sloupce tabulky
**Možnosti:**
*Add column* - Adds a new column to a table
*Drop column* - Deletes a column in a table
*Rename column* - Renames a column
*Modify column* - Changes the data type, size, or constraints of a column
*Add constraint* - Adds a new constraint
*Rename table* - Renames a table
vytvoří tabulku s danýma atributama
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
