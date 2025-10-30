---
title: "Map View Dashboard"
type: "dashboard"
tags: [mapview, dashboard, dataview]
created: 2025-10-23
updated: 2025-10-23
---

# 🗺️ Map View Dashboard

This page lists every note in the vault that has `latitude` and `longitude` in frontmatter.  
Use this as a control center; open a note to see its pin in the **Map View** panel.

> **Tip:** Add `type: settlement | faction | landmark | region_hub` to frontmatter for grouping.

## 📍 Settlements
```dataview
TABLE WITHOUT ID
file.link AS Settlement, latitude, longitude
FROM "04_Settlements"
WHERE latitude AND longitude
SORT file.name ASC
```

## 🛡️ Faction HQs
```dataview
TABLE WITHOUT ID
file.link AS Faction, latitude, longitude
FROM "06_Factions"
WHERE latitude AND longitude
SORT file.name ASC
```

## 🧭 Landmarks (anywhere)
```dataview
TABLE WITHOUT ID
file.link AS Note, type, latitude, longitude
WHERE latitude AND longitude
SORT file.name ASC
```

## 🔎 Missing Coordinates (to fix)
```dataview
TABLE WITHOUT ID
file.link AS Note, type
WHERE (type = "settlement" OR type = "faction" OR contains(tags, "landmark")) AND (latitude = null OR longitude = null)
SORT file.name ASC
```
