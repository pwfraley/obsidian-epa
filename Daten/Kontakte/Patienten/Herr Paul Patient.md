---
anrede: Herr
titel: 
vorname: Paul P.
nachname: Patient
geburtsdatum: 1980-01-16
anschrift:
  straße: Patientenstraße 1
  plz: 11111
  ort: Stadt
  bundesland: Schleswig-Holstein
telefon:
  festnetz: +49 555 555 55 55
  mobil: +49 176 555 55 55
cssclasses:
  - full-width
  - wide-table
---

|              |                                                                                                      | 
| ------------ | ---------------------------------------------------------------------------------------------------- |
| Name:        | `=this.anrede` `=this.titel` `=this.vorname` `=this.nachname`                                        |
| Geburtsdatum | `=this.geburtsdatum`                                                                                 |
| Anschrift    | `=this.anschrift.straße`, `=this.anschrift.plz` `=this.anschrift.ort` - `=this.anschrift.bundesland` |
| Telefon      | `=this.telefon.festnetz`                                                                             |
| Mobil        | `=this.telefon.mobil`                                                                                |
