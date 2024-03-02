---
name: Praxis Dr. Andrea Tilse und Dr. Björn Tilse
anschrift:
  straße: Königstr. 12
  plz: 23552
  ort: Lübeck
telefon: 
  - "+49 451 71042"
fax:
  - "+49 451 71070"
cssclasses:
  - wide-table
  - full-width
---

## `=this.name`

| Infos     | #                                                                     | 
| --------- | --------------------------------------------------------------------- |
| Anschrift | `=this.anschrift.straße`, `=this.anschrift.plz` `=this.anschrift.ort` |
| Telefon   | `=this.telefon`                                                       |
| Fax       | `=this.fax`                                                           |

```dataview
TABLE WITHOUT id
  file.link AS "Praktizierende Ärzte"
FROM "Daten/Kontakte/Ärzte"
WHERE typeof(praxen) = "array" AND contains(praxen, this.file.link)
SORT file.name
```

## Notizen
