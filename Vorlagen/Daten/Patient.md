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

|              |                                                                                                      | 
| ------------ | ---------------------------------------------------------------------------------------------------- |
| Name:        | `=this.anrede` `=this.titel` `=this.vorname` `=this.nachname`                                        |
| Geburtsdatum | `=this.geburtsdatum`                                                                                 |
| Anschrift    | `=this.anschrift.straße`, `=this.anschrift.plz` `=this.anschrift.ort` - `=this.anschrift.bundesland` |
| Telefon      | `=this.telefon.festnetz`                                                                             |
| Mobil        | `=this.telefon.mobil`                                                                                |
