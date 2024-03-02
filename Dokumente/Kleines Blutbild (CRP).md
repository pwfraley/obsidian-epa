---
cssclasses:
  - wide-table
  - full-width
typ: Labor
art: Diagnostik
einstelldatum: 2024-02-26
einsteller:
  - "[[Frau Dr. Andrea Arzt|Frau Dr. Andrea Arzt]]"
erstelldatum: 2024-02-14
autoren:
  - "[[Herr Dr. Alexander Arzt|Herr Dr. Alexander Arzt]]"
fachrichtungen:
  - "[[Daten/Fachrichtungen/LABOR.md|LABOR]]"
befund:
  werte:
    ery: 5,2
    ery_unit: Mio/µl
    leu: 6
    leu_unit: µl
    thr: 25000
    thr_unit: µl
    hb: 16 (10,3)
    hb_unit: g/dl (mmol/l)
    hk: 48
    hk_unit: "%"
    mch: 31
    mch_unit: pg
    mcv: 89
    mcv_unit: fl
    mchc: 32
    mchc_unit: g/dl
patient:
  - "[[Herr Paul Patient|Herr Paul Patient]]"
---

## `=this.typ` Befund (`=this.file.name`)

| Parameter    | Wert                                                 | Einheit                                                   |
| ------------ | ---------------------------------------------------- | --------------------------------------------------------- |
| Erythrozyten | `INPUT[text(class('full-width')):befund.werte.ery]`  | `INPUT[text(class('full-width')):befund.werte.ery_unit]`  |
| Leukozyten   | `INPUT[text(class('full-width')):befund.werte.leu]`  | `INPUT[text(class('full-width')):befund.werte.leu_unit]`  |
| Thrombozyten | `INPUT[text(class('full-width')):befund.werte.thr]`  | `INPUT[text(class('full-width')):befund.werte.thr_unit]`  |
| Hämoglobin   | `INPUT[text(class('full-width')):befund.werte.hb]`   | `INPUT[text(class('full-width')):befund.werte.hb_unit]`   |
| Hämatokrit   | `INPUT[text(class('full-width')):befund.werte.hk]`   | `INPUT[text(class('full-width')):befund.werte.hk_unit]`   |
| MCH          | `INPUT[text(class('full-width')):befund.werte.mch]`  | `INPUT[text(class('full-width')):befund.werte.mch_unit]`  |
| MCV          | `INPUT[text(class('full-width')):befund.werte.mcv]`  | `INPUT[text(class('full-width')):befund.werte.mcv_unit]`  |
| MCHC         | `INPUT[text(class('full-width')):befund.werte.mchc]` | `INPUT[text(class('full-width')):befund.werte.mchc_unit]` |

## Anmerkungen
Es wurden keine Auffälligkeiten festgestellt.  Die Werte sind alle, in dem Alter des Patienten entsprechenden Bereichen.

## Meta

| Prameter        | Wert                                                                             |
| --------------- | -------------------------------------------------------------------------------- |
| Fachrichtungen  | `INPUT[inlineListSuggester(optionQuery("Daten/Fachrichtungen")):fachrichtungen]` | 
| Typ             | `INPUT[text(class('full-width')):typ]`                                           |
| Art             | `INPUT[text(class('full-width')):art]`                                           |
| Erstellt am     | `INPUT[datePicker:erstelldatum]`                                                 |
| Autoren         | `INPUT[inlineListSuggester(optionQuery("Daten/Kontakte/Ärzte")):autoren]`        |
| Eingestellt am  | `INPUT[datePicker:einstelldatum]`                                                |
| Eingestellt von | `INPUT[inlineListSuggester(optionQuery("Daten/Kontakte")):einsteller]`           |
| Patient         | `INPUT[inlineListSuggester(optionQuery("Daten/Kontakte/Patienten")):patient]`    |
