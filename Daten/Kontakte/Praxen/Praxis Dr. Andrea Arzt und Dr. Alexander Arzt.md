---
name: Praxis Dr. Andrea Arzt und Dr. Alexander Arzt
fachrichtungen:
  - "[[Daten/Fachrichtungen/ALLGEMEIN.md|ALLGEMEIN]]"
anschrift:
  straße: Ärztestr. 12
  plz: 11111
  ort: Stadt
telefon:
  - +49 555 555
fax:
  - +49 555 554
cssclasses:
  - wide-table
  - full-width
---

## `=this.name`

| Infos          | #                                                                                |
| -------------- | -------------------------------------------------------------------------------- |
| Fachrichtungen | `INPUT[inlineListSuggester(optionQuery("Daten/Fachrichtungen")):fachrichtungen]` |
| Anschrift      | `=this.anschrift.straße`, `=this.anschrift.plz` `=this.anschrift.ort`            |
| Telefon        | `=this.telefon`                                                                  |
| Fax            | `=this.fax`                                                                      |

```dataview
TABLE WITHOUT id
  file.link AS "Praktizierende Ärzte"
FROM "Daten/Kontakte/Ärzte"
WHERE typeof(praxen) = "array" AND contains(praxen, this.file.link)
SORT file.name
```

## Notizen
