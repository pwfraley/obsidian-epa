---
anrede: 
titel: 
vorname: 
nachname: 
geburtsdatum: 
anschrift:
  straße: 
  plz: 
  ort: 
  bundesland: 
telefon:
  festnetz: 
  mobil: 
cssclasses:
  - full-width
  - wide-table
---

## `=this.anrede` `=this.titel` `=this.vorname` `=this.nachname`

|              |                                                                                                      | 
| ------------ | ---------------------------------------------------------------------------------------------------- |
| Name:        | `=this.anrede` `=this.titel` `=this.vorname` `=this.nachname`                                        |
| Geburtsdatum | `=this.geburtsdatum`                                                                                 |
| Anschrift    | `=this.anschrift.straße`, `=this.anschrift.plz` `=this.anschrift.ort` - `=this.anschrift.bundesland` |
| Telefon      | `=this.telefon.festnetz`                                                                             |
| Mobil        | `=this.telefon.mobil`                                                                                |

## Letzte Untersuchungen

```dataview
TABLE without id
  typ AS "Typ",
  art AS "Art",
  file.link AS "Bezeichnung",
  erstelldatum AS "Erstelldatum",
  autoren AS "Autoren",
  fachrichtungen AS "Fachrichtungen"
FROM "Dokumente"
WHERE contains(patient, this.file.link)
SORT einstelldatum DESC LIMIT 10
```
