---
name: 
anschrift:
  straße: 
  plz: 
  ort: 
telefon: []
fax: []
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
