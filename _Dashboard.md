---
created: 2026-05-16
basis: primary-source
tags:
  - dashboard
---

# Vault Dashboard

## Basis Audit — Needs Attention

### TBD (source not yet assigned)
```dataview
TABLE file.folder AS "Folder", created
FROM "Coaching" OR "Coaching Clients" OR "Coaching Me" OR "Articles"
WHERE basis = "TBD"
SORT file.mtime DESC
```

### Missing basis field entirely
```dataview
TABLE file.folder AS "Folder", file.mtime AS "Modified"
FROM "Coaching" OR "Coaching Clients" OR "Coaching Me" OR "Articles"
WHERE !basis
SORT file.mtime DESC
```

## Recent Activity — Last 7 Days
```dataview
TABLE file.folder AS "Folder", basis, file.mtime AS "Modified"
FROM "Coaching" OR "Coaching Clients" OR "Coaching Me" OR "Articles"
WHERE file.mtime >= date(today) - dur(7 days)
SORT file.mtime DESC
```

## Clients
```dataview
TABLE created, file.mtime AS "Last Session"
FROM "Coaching Clients"
SORT file.mtime DESC
```

## Practitioner References
```dataview
TABLE basis, created
FROM "Coaching/Disciple Fit Covenant Identity Coaching Prep/06 — Practitioner Reference"
SORT created DESC
```

## Pending Tasks
```dataview
TASK
WHERE !completed
FROM "Coaching" OR "Coaching Clients" OR "Coaching Me" OR "Articles"
SORT file.mtime DESC
```
