---
created: 2026-10-13
basis: "[[Covenant Identity — System Document Master List]] — the curated, annotated inventory this page complements. Rebuilt 2026-10-13 as a live Dataview index, replacing a static one-sentence-per-file list that had been edited twice (2026-09-16 and 2026-10-07) and was missing about 123 files when audited. Design choice made by Andrew 2026-10-13. One-sentence descriptions of each file are kept in Claude's memory index (covenant_identity_file_index), which sits outside the vault."
tags:
  - index
  - navigation
  - live
---

# Covenant Identity Coaching Prep — File Index

*Live index. Every table on this page is a Dataview query, so it updates by itself when a file is created, renamed, or moved. Nothing needs to be added here by hand.*

> [!tip] Live Pages — Quick Access
> 🔗 **[Covenant Identity Coaching — Foundation, Mechanism & Distinctives](https://claude.ai/code/artifact/05d05db3-fc9c-457d-bf5a-c68d8e2507b5)** — Peer Practitioner Briefing companion page
> 🔗 **[Witnessing Repentance — Session Guide](https://claude.ai/code/artifact/b532cd10-2315-4eb4-ba77-667ba39225ae)** — in-session coach tool

---

## How This Page Works

- Each table lists the notes in one folder, sorted by file name. In `04 — Session Tools` and `08 — Between-Session Materials`, the deployment code at the front of each name (ALLa, P1a, P2-3a, and so on) makes the name sort follow usage order.
- This page shows **what exists**. It carries no descriptions. For annotated entries, use the [[Covenant Identity — System Document Master List]] (every document, with status and description), the [[Covenant Identity — Document Reading Order]] (the sequence to read them in), and the [[Covenant Identity — Practitioner Reference Index]] (the diagnostic and theoretical cluster).
- A table that says "No results" has nothing in that folder. If every table is empty, check that the Dataview plugin is enabled.
- A new **top-level folder** in this track needs a new section here. The "Anything not listed above" check at the bottom catches it: that table should always be empty.

---

## Completeness Check

### Total files in this track
```dataview
TABLE WITHOUT ID length(rows) AS "Files in this track (including this page)"
FROM "Coaching/Covenant Identity Coaching Prep"
GROUP BY true
```

### Files per folder
```dataview
TABLE WITHOUT ID choice(key = "Coaching/Covenant Identity Coaching Prep", "(top of the track)", replace(key, "Coaching/Covenant Identity Coaching Prep/", "")) AS "Folder", length(rows) AS "Files"
FROM "Coaching/Covenant Identity Coaching Prep"
GROUP BY file.folder
SORT key ASC
```

### Recently added (last 14 days, by the `created` field)
```dataview
TABLE WITHOUT ID file.link AS "Document", created AS "Created", choice(file.folder = "Coaching/Covenant Identity Coaching Prep", "(top of the track)", replace(file.folder, "Coaching/Covenant Identity Coaching Prep/", "")) AS "Folder"
FROM "Coaching/Covenant Identity Coaching Prep"
WHERE created AND created >= date(today) - dur(14 days) AND file.path != this.file.path
SORT created DESC, file.name ASC
```

---

## Root
*Navigation hubs, the master list, the reading order, and loose files at the top of the track.*
```dataview
TABLE WITHOUT ID file.link AS "Document", created AS "Created", file.mtime AS "Modified"
FROM "Coaching/Covenant Identity Coaching Prep"
WHERE file.folder = "Coaching/Covenant Identity Coaching Prep" AND file.path != this.file.path
SORT file.name ASC
```

---

## 01 — Model Foundation
*Includes the `Support Documents for Model Foundation` subfolder.*
```dataview
TABLE WITHOUT ID file.link AS "Document", replace(file.folder, "Coaching/Covenant Identity Coaching Prep/01 — Model Foundation", "") AS "Subfolder", created AS "Created", file.mtime AS "Modified"
FROM "Coaching/Covenant Identity Coaching Prep/01 — Model Foundation"
SORT file.name ASC
```

---

## 02 — Client Onboarding
```dataview
TABLE WITHOUT ID file.link AS "Document", created AS "Created", file.mtime AS "Modified"
FROM "Coaching/Covenant Identity Coaching Prep/02 — Client Onboarding"
SORT file.name ASC
```

---

## 03 — Intake System
```dataview
TABLE WITHOUT ID file.link AS "Document", created AS "Created", file.mtime AS "Modified"
FROM "Coaching/Covenant Identity Coaching Prep/03 — Intake System"
SORT file.name ASC
```

---

## 04 — Session Tools
*Deployment codes: ALL (every session), DC (Discovery Call), P1–P4 (phases), P2-3 (spans late Phase 2 into Phase 3).*
```dataview
TABLE WITHOUT ID file.link AS "Document", created AS "Created", file.mtime AS "Modified"
FROM "Coaching/Covenant Identity Coaching Prep/04 — Session Tools"
SORT file.name ASC
```

---

## 05 — Growth Tracking
```dataview
TABLE WITHOUT ID file.link AS "Document", created AS "Created", file.mtime AS "Modified"
FROM "Coaching/Covenant Identity Coaching Prep/05 — Growth Tracking"
SORT file.name ASC
```

---

## 06 — Practitioner Reference
*Includes the `Co-Regulation Skill Development` and `Sanctification Module — The Believer's Part` subfolders. The Subfolder column is blank for files at the top of the folder.*
```dataview
TABLE WITHOUT ID file.link AS "Document", replace(file.folder, "Coaching/Covenant Identity Coaching Prep/06 — Practitioner Reference", "") AS "Subfolder", created AS "Created", file.mtime AS "Modified"
FROM "Coaching/Covenant Identity Coaching Prep/06 — Practitioner Reference"
SORT file.name ASC
```

---

## 07 — AI Prompts
```dataview
TABLE WITHOUT ID file.link AS "Document", created AS "Created", file.mtime AS "Modified"
FROM "Coaching/Covenant Identity Coaching Prep/07 — AI Prompts"
SORT file.name ASC
```

---

## 08 — Between-Session Materials
*Deployment codes: ALL (every client), P1 and P2a–P2l (by phase and scenario), P3 (Phase 3).*
```dataview
TABLE WITHOUT ID file.link AS "Document", created AS "Created", file.mtime AS "Modified"
FROM "Coaching/Covenant Identity Coaching Prep/08 — Between-Session Materials"
SORT file.name ASC
```

---

## 09 — Resource Library
```dataview
TABLE WITHOUT ID file.link AS "Document", created AS "Created", file.mtime AS "Modified"
FROM "Coaching/Covenant Identity Coaching Prep/09 — Resource Library"
SORT file.name ASC
```

---

## Practitioner Development
*Folder-level membership is also tracked in [[Covenant Identity — Practitioner Development — Index]].*
```dataview
TABLE WITHOUT ID file.link AS "Document", created AS "Created", file.mtime AS "Modified"
FROM "Coaching/Covenant Identity Coaching Prep/Practitioner Development"
SORT file.name ASC
```

---

## Lesson Drafts
*Drafting material for lessons, not part of the practitioner reading set.*
```dataview
TABLE WITHOUT ID file.link AS "Document", created AS "Created", file.mtime AS "Modified"
FROM "Coaching/Covenant Identity Coaching Prep/Lesson Drafts"
SORT file.name ASC
```

---

## Anything not listed above
*This table should always be empty. If a file appears here, it sits in a folder that has no section on this page yet. Add a section for that folder.*
```dataview
TABLE WITHOUT ID file.link AS "Document", file.folder AS "Folder"
FROM "Coaching/Covenant Identity Coaching Prep"
WHERE file.folder != "Coaching/Covenant Identity Coaching Prep"
AND !startswith(file.folder, "Coaching/Covenant Identity Coaching Prep/01 — Model Foundation")
AND !startswith(file.folder, "Coaching/Covenant Identity Coaching Prep/02 — Client Onboarding")
AND !startswith(file.folder, "Coaching/Covenant Identity Coaching Prep/03 — Intake System")
AND !startswith(file.folder, "Coaching/Covenant Identity Coaching Prep/04 — Session Tools")
AND !startswith(file.folder, "Coaching/Covenant Identity Coaching Prep/05 — Growth Tracking")
AND !startswith(file.folder, "Coaching/Covenant Identity Coaching Prep/06 — Practitioner Reference")
AND !startswith(file.folder, "Coaching/Covenant Identity Coaching Prep/07 — AI Prompts")
AND !startswith(file.folder, "Coaching/Covenant Identity Coaching Prep/08 — Between-Session Materials")
AND !startswith(file.folder, "Coaching/Covenant Identity Coaching Prep/09 — Resource Library")
AND !startswith(file.folder, "Coaching/Covenant Identity Coaching Prep/Practitioner Development")
AND !startswith(file.folder, "Coaching/Covenant Identity Coaching Prep/Lesson Drafts")
SORT file.folder ASC, file.name ASC
```
