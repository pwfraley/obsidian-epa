---
cssClass: "wide-table"
---
## Patient

```dataview
TABLE without id
  anrede AS "Anrede",
  titel AS "Titel",
  vorname AS "Vorname",
  nachname AS "Nachname",
  geburtsdatum AS "Geburtsdatum"
FROM "Daten/Kontakte/Patienten"
LIMIT 1
```

## Letzte Untersuchungen

```dataview
TABLE without id
  typ AS "Typ",
  art AS "Art",
  file.link AS "Bezeichnung",
  erstelldatum AS "Erstelldatum",
  autoren AS "Autoren",
  fachrichtung AS "Fachrichtung"
FROM "Dokumente"
SORT einstelldatum DESC LIMIT 5
```
