---
{"dg-publish":true,"permalink":"/dbs-seznam-poznamek/","dg-note-properties":{}}
---


```base
views:
  - type: table
    name: Table
    filters:
      and:
        - note["cards-deck"] == "DBS"
    order:
      - file.name
      - file.tags
      - is-in-anki?
      - file.ctime
    sort:
      - property: is-in-anki?
        direction: ASC

```
