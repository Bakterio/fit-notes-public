---
{"dg-publish":true,"permalink":"/dbs-seznam-poznamek/","dg-note-properties":{}}
---


```base
views:
  - type: table
    name: Table
    filters:
      and:
        - note["dg-publish"] == true
        - note["cards-deck"] == "DBS"
        - file.ext == "md"
    sort:
      - property: file.name
        direction: ASC

```

