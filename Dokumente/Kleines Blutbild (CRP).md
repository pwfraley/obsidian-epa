---
cssclasses:
  - wide-table
  - full-width
typ: Labor
art: Diagnostik
einstelldatum: 2024-02-26
einsteller:
  - "[[Daten/Kontakte/Ärzte/Frau Dr. Andrea Tilse.md|Frau Dr. Andrea Tilse]]"
erstelldatum: 2024-02-14
autoren:
  - "[[Daten/Kontakte/Ärzte/Herr Dr. Björn Tilse.md|Herr Dr. Björn Tilse]]"
fachrichtung: "[[LABOR]]"
befund:
  werte:
    ery: 4,5–5,9 Mio/µl
    leu: 4.000–10.000/µl
    thr: 150000–350000/µl
    hb: 14–18 g/dl (8,7–11,2 mmol/l)
    hk: 41–50 %
    mch: 27–34 pg
    mcv: 85–98 fl
    mchc: 30–36 g/dl
---

## `=this.typ` Befund (`=this.file.name`)

| Parameter    | Wert                                                   |
| ------------ | ------------------------------------------------------ |
| Erythrozyten | `INPUT[text(class('full-width')):befund.werte.ery]`    |
| Leukozyten   | `INPUT[text(class('full-width')):befund.werte.leu]`    |
| Thrombozyten | `INPUT[text(class('full-width')):befund.werte.thr]`    |
| Hämoglobin   | `INPUT[textArea(class('full-width')):befund.werte.hb]` |
| Hämatokrit   | `INPUT[text(class('full-width')):befund.werte.hk]`     |
| MCH          | `INPUT[text(class('full-width')):befund.werte.mch]`    |
| MCV          | `INPUT[text(class('full-width')):befund.werte.mcv]`    |
| MCHC         | `INPUT[text(class('full-width')):befund.werte.mchc]`   | 

## Anmerkungen
Es wurden keine Auffälligkeiten festgestellt.  Die Werte sind alle, in dem Alter des Patienten entsprechenden Bereichen.

## Meta

| Prameter        | Wert                                                                      | 
| --------------- | ------------------------------------------------------------------------- |
| Typ             | `INPUT[text(class('full-width')):typ]`                                    |
| Art             | `INPUT[text(class('full-width')):art]`                                    |
| Erstellt am     | `INPUT[datePicker:erstelldatum]`                                          |
| Autoren         | `INPUT[inlineListSuggester(optionQuery("Daten/Kontakte/Ärzte")):autoren]` |
| Eingestellt am  | `INPUT[datePicker:einstelldatum]`                                         |
| Eingestellt von | `INPUT[inlineListSuggester(optionQuery("Daten/Kontakte")):einsteller]`    |
