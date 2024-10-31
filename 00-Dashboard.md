---
cssclasses:
  - wide-table
  - full-width
---
## Patienten

```dataview
TABLE without id
  file.link AS "Name",
  geburtsdatum AS "Geburtsdatum"
FROM "Daten/Kontakte/Patienten"
```

## Termine

```dataview
TABLE without id
  typ AS "Typ",
  art AS "Art",
  file.link AS "Bezeichnung",
  erstelldatum AS "Erstelldatum",
  autoren AS "Autoren",
  fachrichtungen AS "Fachrichtungen"
FROM "Termine"
SORT einstelldatum DESC LIMIT 5
```

## Neueste Dokumente

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
