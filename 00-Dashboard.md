---
cssclasses:
  - wide-table
  - full-width
---
## Patient

```dataview
TABLE without id
  file.link AS "Name",
  geburtsdatum AS "Geburtsdatum"
FROM "Daten/Kontakte/Patienten"
```

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
SORT einstelldatum DESC LIMIT 5
```
