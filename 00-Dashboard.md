---
cssClass: "wide-table"
---

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
