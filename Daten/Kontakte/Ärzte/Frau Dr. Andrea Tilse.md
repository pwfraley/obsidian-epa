---
anrede: Frau
titel: Dr.
vorname: Andrea
nachname: Tilse
beruf: Fachärztin für Allgemeinmedizin
praxen:
  - "[[Daten/Kontakte/Praxen/Praxis Dr. Andrea Tilse und Dr. Björn Tilse.md|Praxis Dr. Andrea Tilse und Dr. Björn Tilse]]"
anschrift:
  straße: Königstr. 12
  plz: 23552
  ort: Lübeck
telefon:
  - +49 451 71042
fax:
  - +49 451 71070
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
