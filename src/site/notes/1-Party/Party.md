---
{"dg-publish":true,"permalink":"/1-party/party/","tags":["gardenEntry"],"noteIcon":""}
---


| Player                                            | HP | Class                                | Race                         | Level | AC | Pass Perc (WIS) |
| ------------------------------------------------- | -- | ------------------------------------ | ---------------------------- | ----- | -- | --------------- |
| [[1-Party/Hadiel\|Hadiel]]                     | 15 | <ul><li>Cleric</li></ul>             | <ul><li>Changeling</li></ul> | 2     | 17 | 13              |
| [[1-Party/Osama d. pluh\|Osama d. pluh]]       | 18 | <ul><li>Warlock</li></ul>            | <ul><li>Dragonborn</li></ul> | 2     | 13 | 10              |
| [[1-Party/Senshi Greybeard\|Senshi Greybeard]] | 17 | <ul><li>Bard</li><li>Rogue</li></ul> | <ul><li>Dwarf</li></ul>      | 2     | 14 | 12              |

{ .block-language-dataview}
```base
properties:
  note.level:
    displayName: Level
  note.hp:
    displayName: HP
  note.ac:
    displayName: AC
  note.pasperc:
    displayName: Pass Perc (WIS)
views:
  - type: table
    name: Table
    filters:
      and:
        - file.path.startsWith("1-Party")
        - Role == "Player"
    order:
      - file.name
      - hp
      - Class
      - Race
      - level
      - ac
      - pasperc
    sort: []
    columnSize:
      file.name: 554

```
