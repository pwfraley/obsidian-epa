---
anrede: 
titel: 
vorname: 
nachname: 
beruf: 
praxen: []
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

|           |                                                                           |
| --------- | ------------------------------------------------------------------------- |
| Name:     | `=this.anrede` `=this.titel` `=this.vorname` `=this.nachname`             |
| Praxis    | `INPUT[inlineListSuggester(optionQuery("Daten/Kontakte/Praxen")):praxen]` | 
| Anschrift | `=this.anschrift.straße`, `=this.anschrift.plz` `=this.anschrift.ort`     |
| Telefon   | `=this.telefon`                                                           |
| Fax       | `=this.fax`                                                               |

## Notizen
