---
anrede: Herr
titel: Dr.
vorname: Alexander
nachname: Arzt
beruf: Facharzt für Allgemeinmedizin
fachrichtungen:
  - "[[Daten/Fachrichtungen/ALLGEMEIN.md|ALLGEMEIN]]"
praxen:
  - "[[Praxis Dr. Andrea Arzt und Dr. Alexander Arzt|Praxis Dr. Andrea Arzt und Dr. Alexander Arzt]]"
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

|                |                                                                                  |
| -------------- | -------------------------------------------------------------------------------- |
| Name:          | `=this.anrede` `=this.titel` `=this.vorname` `=this.nachname`                    |
| Fachrichtungen | `INPUT[inlineListSuggester(optionQuery("Daten/Fachrichtungen")):fachrichtungen]` |
| Praxis         | `INPUT[inlineListSuggester(optionQuery("Daten/Kontakte/Praxen")):praxen]`        |
| Anschrift      | `=this.anschrift.straße`, `=this.anschrift.plz` `=this.anschrift.ort`            |
| Telefon        | `=this.telefon`                                                                  |
| Fax            | `=this.fax`                                                                      |

## Notizen
