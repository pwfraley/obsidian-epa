---
cssclasses:
  - wide-table
  - full-width
typ: Labor
art: Diagnostik
einstelldatum: <% tp.file.creation_date() %>
einsteller: []
erstelldatum: 
autoren: []
fachrichtungen:
  - "[[Daten/Fachrichtungen/LABOR.md|LABOR]]"
befund:
  werte:
    ery: 
    ery_unit: Mio/µl
    leu: 
    leu_unit: µl
    thr: 
    thr_unit: µl
    hb: 
    hb_unit: g/dl (mmol/l)
    hk: 
    hk_unit: "%"
    mch: 
    mch_unit: pg
    mcv: 
    mcv_unit: fl
    mchc: 
    mchc_unit: g/dl
icon: ":FasDroplet:"
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
