---
created: 2026-05-26
basis: "[[Relational Performance Advisory — Multi-Rater 360 Instrument]] — clusters, items, scoring protocol, divergence flag spec"
tags:
  - rpa
  - advisory
  - assessment
  - 360
  - google-sheets
  - template
---

# Relational Performance Advisory — 360 Scoring Template Design

**What this is:** Build instructions for the Google Sheets scoring template. Follow this document to build the template once; duplicate it per engagement. No coding required — only formulas.

**Tools required:** Google Forms (two forms: one rater survey, one self-rating survey) + Google Sheets (one workbook per engagement, linked to both forms).

**Time to build:** 2–3 hours for the initial template. Duplicating for a new engagement: 15 minutes.

---

## Overview — Five Tabs

| Tab | Purpose | Who populates it |
|---|---|---|
| **Raw_Rater** | All rater responses from the rater survey | Google Forms (automatic) |
| **Raw_Self** | All self-rating responses from the self-rating survey | Google Forms (automatic) |
| **Calc_Rater** | Per-rater cluster means (helper) | Formulas — drag down as responses arrive |
| **Scoring_Table** | Group means, self-rating, divergence flags — one block per leader | Formulas — add a new block per leader |
| **Open_Text** | All open-text responses pulled by leader | Formulas — add a new section per leader |

---

## Google Forms Setup

### Form 1 — Rater Survey
Create a Google Form linked to the Raw_Rater tab. Field order matters — the column positions in Raw_Rater depend on it.

**Field order:**

| Position | Question | Type |
|---|---|---|
| 1 | Timestamp | Auto (col A) |
| 2 | Leader Name | Dropdown — list all leaders by name (col B) |
| 3 | Your relationship to this leader | Multiple choice: Supervisor / Peer / Direct Report (col C) |
| 4 | How long have you worked with this leader? | Multiple choice: <6 mo / 6–12 mo / 1–3 yr / 3+ yr (col D) |
| 5–9 | Items 1.1–1.5 (Accountability Delivery) | Linear scale 1–5 (cols E–I) |
| 10–14 | Items 2.1–2.5 (Regulation Under Pressure) | Linear scale 1–5 (cols J–N) |
| 15–19 | Items 3.1–3.5 (Feedback Receptivity) | Linear scale 1–5 (cols O–S) |
| 20–24 | Items 4.1–4.5 (Relational Repair) | Linear scale 1–5 (cols T–X) |
| 25–29 | Items 5.1–5.5 (Authority Clarity) | Linear scale 1–5 (cols Y–AC) |
| 30–34 | Open-text prompts (one per cluster) | Paragraph (cols AD–AH) |

**N/O handling:** Use a linear scale (1–5) and add this instruction at the top of each cluster section: *"Leave blank if you have not had the opportunity to observe this behavior."* Blank responses are automatically excluded from AVERAGE calculations in Sheets — no special handling needed.

**Label the scale ends:** 1 = Never observed, 5 = Consistently observed.

### Form 2 — Self-Rating Survey
Separate Google Form linked to the Raw_Self tab. No rater relationship field — just leader name and the 25 items.

**Field order:**

| Position | Question | Type |
|---|---|---|
| 1 | Timestamp | Auto (col A) |
| 2 | Your name | Dropdown — same leader list (col B) |
| 3–7 | Items 1.1–1.5 | Linear scale 1–5 (cols C–G) |
| 8–12 | Items 2.1–2.5 | Linear scale 1–5 (cols H–L) |
| 13–17 | Items 3.1–3.5 | Linear scale 1–5 (cols M–Q) |
| 18–22 | Items 4.1–4.5 | Linear scale 1–5 (cols R–V) |
| 23–27 | Items 5.1–5.5 | Linear scale 1–5 (cols W–AA) |

No open-text fields on the self-rating form.

---

## Tab 1 — Raw_Rater

Auto-populated by Google Forms. Do not edit this tab manually.

**Expected columns after Forms links:**

| Col | Content |
|---|---|
| A | Timestamp |
| B | Leader Name |
| C | Rater Relationship |
| D | Tenure |
| E–I | Items 1.1–1.5 (Accountability Delivery) |
| J–N | Items 2.1–2.5 (Regulation Under Pressure) |
| O–S | Items 3.1–3.5 (Feedback Receptivity) |
| T–X | Items 4.1–4.5 (Relational Repair) |
| Y–AC | Items 5.1–5.5 (Authority Clarity) |
| AD | Open text — Accountability Delivery |
| AE | Open text — Regulation Under Pressure |
| AF | Open text — Feedback Receptivity |
| AG | Open text — Relational Repair |
| AH | Open text — Authority Clarity |

**Verify** column positions match after linking Forms. If Forms adds or reorders fields, update column references in Calc_Rater accordingly.

---

## Tab 2 — Raw_Self

Auto-populated by the self-rating Google Form. Do not edit manually.

| Col | Content |
|---|---|
| A | Timestamp |
| B | Leader Name |
| C–G | Items 1.1–1.5 |
| H–L | Items 2.1–2.5 |
| M–Q | Items 3.1–3.5 |
| R–V | Items 4.1–4.5 |
| W–AA | Items 5.1–5.5 |

---

## Tab 3 — Calc_Rater

**Purpose:** Converts raw item scores into per-rater cluster means. Scoring_Table formulas pull from here.

**Row 1 — Headers (type these manually):**

| Col | Header |
|---|---|
| A | Timestamp |
| B | Leader |
| C | Relationship |
| D | C1 — Accountability |
| E | C2 — Regulation |
| F | C3 — Receptivity |
| G | C4 — Repair |
| H | C5 — Authority |

**Row 2 — Formulas (enter these, then drag down to row 200):**

| Col | Formula |
|---|---|
| A2 | `=IF(Raw_Rater!A2="","",Raw_Rater!A2)` |
| B2 | `=IF(Raw_Rater!B2="","",Raw_Rater!B2)` |
| C2 | `=IF(Raw_Rater!C2="","",Raw_Rater!C2)` |
| D2 | `=IFERROR(AVERAGE(Raw_Rater!E2,Raw_Rater!F2,Raw_Rater!G2,Raw_Rater!H2,Raw_Rater!I2),"")` |
| E2 | `=IFERROR(AVERAGE(Raw_Rater!J2,Raw_Rater!K2,Raw_Rater!L2,Raw_Rater!M2,Raw_Rater!N2),"")` |
| F2 | `=IFERROR(AVERAGE(Raw_Rater!O2,Raw_Rater!P2,Raw_Rater!Q2,Raw_Rater!R2,Raw_Rater!S2),"")` |
| G2 | `=IFERROR(AVERAGE(Raw_Rater!T2,Raw_Rater!U2,Raw_Rater!V2,Raw_Rater!W2,Raw_Rater!X2),"")` |
| H2 | `=IFERROR(AVERAGE(Raw_Rater!Y2,Raw_Rater!Z2,Raw_Rater!AA2,Raw_Rater!AB2,Raw_Rater!AC2),"")` |

Select A2:H2. Drag the selection down to row 200. New form responses auto-populate Raw_Rater; Calc_Rater picks them up immediately.

---

## Tab 4 — Scoring_Table

**Purpose:** The main working output. One block per leader. All divergence flags appear here.

### Block Structure

Each leader gets a 9-row block. Repeat the structure for each leader, leaving one blank row between blocks.

**Block for Leader 1 — starting at row 2:**

| Row | Col A | Col B | Col C | Col D | Col E | Col F | Col G | Col H | Col I |
|---|---|---|---|---|---|---|---|---|---|
| 2 | **LEADER NAME** | *(type name here)* | | | | | | | |
| 3 | *(blank)* | **Supervisor** | **Peer** | **Direct Report** | **All-Rater** | **Self** | **Divergence** | **Flag** | **N (raters)** |
| 4 | Accountability Delivery | formula | formula | formula | formula | formula | formula | formula | formula |
| 5 | Regulation Under Pressure | formula | formula | formula | formula | formula | formula | formula | formula |
| 6 | Feedback Receptivity | formula | formula | formula | formula | formula | formula | formula | formula |
| 7 | Relational Repair | formula | formula | formula | formula | formula | formula | formula | formula |
| 8 | Authority Clarity | formula | formula | formula | formula | formula | formula | formula | formula |
| 9 | *(blank separator)* | | | | | | | | |

**In B2, type the leader's name.** All formulas in the block reference `$B$2` — change the name in B2 and the entire block recalculates for that leader.

### Formulas — Accountability Delivery Row (Row 4)

The cluster column in Calc_Rater for Accountability Delivery is **D**. Substitute E, F, G, H for the other clusters in rows 5–8.

**B4 — Supervisor Mean:**
```
=IFERROR(AVERAGEIFS(Calc_Rater!D:D,Calc_Rater!B:B,$B$2,Calc_Rater!C:C,"Supervisor"),"–")
```

**C4 — Peer Mean:**
```
=IFERROR(AVERAGEIFS(Calc_Rater!D:D,Calc_Rater!B:B,$B$2,Calc_Rater!C:C,"Peer"),"–")
```

**D4 — Direct Report Mean:**
```
=IFERROR(AVERAGEIFS(Calc_Rater!D:D,Calc_Rater!B:B,$B$2,Calc_Rater!C:C,"Direct Report"),"–")
```

**E4 — All-Rater Mean:**
```
=IFERROR(AVERAGEIF(Calc_Rater!B:B,$B$2,Calc_Rater!D:D),"–")
```

**F4 — Self-Rating (pulls from Raw_Self):**
```
=IFERROR(AVERAGEIF(Raw_Self!B:B,$B$2,Raw_Self!C:G),"–")
```
*Note: Raw_Self!C:G covers items 1.1–1.5 (Accountability Delivery). Adjust the range for each cluster row:*
- Accountability Delivery: `Raw_Self!C:G`
- Regulation Under Pressure: `Raw_Self!H:L`
- Feedback Receptivity: `Raw_Self!M:Q`
- Relational Repair: `Raw_Self!R:V`
- Authority Clarity: `Raw_Self!W:AA`

*AVERAGEIF on a multi-column range averages all matching values across the range — this produces the cluster mean from the self-rating form correctly.*

**G4 — Divergence (Self minus All-Rater):**
```
=IFERROR(F4-E4,"–")
```
Positive = self rated higher than raters. Negative = self rated lower.

**H4 — Flag:**
```
=IF(ISNUMBER(G4),IF(ABS(G4)>=2,"⚠ FLAG",""),"")
```

**I4 — Rater Count (N):**
```
=COUNTIF(Calc_Rater!B:B,$B$2)
```
This counts total rater responses for this leader. To count by group (e.g., direct reports only):
```
=COUNTIFS(Calc_Rater!B:B,$B$2,Calc_Rater!C:C,"Direct Report")
```

### Replicating for Other Clusters

In rows 5–8, copy the formulas from row 4 and change only the Calc_Rater column reference and the Raw_Self range:

| Row | Cluster | Calc_Rater col | Raw_Self range |
|---|---|---|---|
| 4 | Accountability Delivery | D | C:G |
| 5 | Regulation Under Pressure | E | H:L |
| 6 | Feedback Receptivity | F | M:Q |
| 7 | Relational Repair | G | R:V |
| 8 | Authority Clarity | H | W:AA |

### Adding a New Leader Block

Start the next block 1 row below the separator. Change `$B$2` to `$B$12` (or wherever the new leader's name cell sits). Copy the entire 9-row block, paste it below, update the name cell reference in all formulas.

**Faster:** Name each leader cell (e.g., name B2 "Leader1", B12 "Leader2"). Then formulas reference the name instead of the cell address — no updating needed when you copy.

### Conditional Formatting

Apply to columns B–E (the four mean columns) across all data rows:

| Rule | Format |
|---|---|
| Value ≤ 2.5 | Red background (low presence — pattern signal) |
| Value 2.6–3.4 | Yellow background (moderate) |
| Value ≥ 3.5 | Green background (collaborative capacity range) |

Apply to column H (Flag):
| Rule | Format |
|---|---|
| Cell contains "FLAG" | Bold red text |

Apply to column G (Divergence):
| Rule | Format |
|---|---|
| Value ≥ 2 | Bold orange (self rated higher — limited self-awareness) |
| Value ≤ -2 | Bold blue (self rated lower — underestimation) |

---

## Tab 5 — Open_Text

**Purpose:** Collects all open-text responses per leader per cluster in one place. Andrew reads these during profile building — not shared with the leader or sponsor.

### Structure

One section per leader. Five clusters per section.

**Section header (type manually):** Leader Name

**Cluster subsections — use FILTER formula to pull all non-blank responses:**

*Accountability Delivery responses for leader in cell A2:*
```
=FILTER(Raw_Rater!AD:AD,(Raw_Rater!B:B=A2)*(Raw_Rater!AD:AD<>""))
```

*Regulation Under Pressure (column AE):*
```
=FILTER(Raw_Rater!AE:AE,(Raw_Rater!B:B=A2)*(Raw_Rater!AE:AE<>""))
```

Repeat for columns AF, AG, AH (clusters 3–5).

**Layout for one leader section:**

Row 1: Leader name (manual)
Row 2: "ACCOUNTABILITY DELIVERY" (header — manual)
Row 3+: FILTER formula — auto-expands as responses arrive
[Blank row]
Next header: "REGULATION UNDER PRESSURE"
...and so on.

**Note on FILTER:** FILTER is a dynamic array formula — it spills results into the rows below. Leave enough blank rows between cluster sections to accommodate the maximum expected number of rater responses (8–10 rows per cluster is safe for a 4–8 leader cohort).

---

## Month 12 Abbreviated Version

The scoring template works identically for the Month 12 abbreviated 360 — same structure, same formulas. The only difference is the form: use only the ★-marked items (15 items, 3 per cluster). Build a separate Google Form (Form 3 — Rater Abbreviated, Form 4 — Self Abbreviated) linked to new raw data tabs (Raw_Rater_M12 and Raw_Self_M12).

Add a second block per leader in Scoring_Table:

```
B2: "Jane Smith — Baseline"     B12: "Jane Smith — Month 12"
```

Add a **Change** column in each Month 12 block:

```
=IFERROR(E_month12 - E_baseline, "–")
```

This produces the pattern movement number for the Month 12 sponsor report.

---

## Setup Checklist

- [ ] Create Rater Survey in Google Forms — all 29 fields in correct order
- [ ] Link Rater Survey to a new Google Sheets workbook — tab named Raw_Rater
- [ ] Create Self-Rating Survey in Google Forms — 27 fields
- [ ] Link Self-Rating Survey to same workbook — tab named Raw_Self
- [ ] Build Calc_Rater tab — headers + row 2 formulas, dragged to row 200
- [ ] Build Scoring_Table tab — one complete leader block built and verified
- [ ] Apply conditional formatting to Scoring_Table
- [ ] Build Open_Text tab — one complete leader section built and verified
- [ ] Test with dummy data — submit one rater response and one self-rating, verify all calculations populate correctly
- [ ] Save this workbook as the master template
- [ ] For each engagement: File → Make a copy → rename with leader cohort and date

---

## Troubleshooting

**Means showing as "–" when responses exist**
Check that the leader name in B2 (Scoring_Table) matches the spelling exactly as entered in the Google Form dropdown. One extra space breaks the AVERAGEIF match.

**FILTER formula showing #N/A**
No responses yet for that leader/cluster combination. Wrap in IFERROR: `=IFERROR(FILTER(...),"No responses yet")`

**Self-rating pulling wrong cluster**
Verify the Raw_Self column range matches the correct cluster. Items 1.1–1.5 start at column C (third column) since columns A and B are Timestamp and Leader Name.

**Rater count (N) looks wrong**
COUNTIF counts all rows with that leader name, including the header row if the name accidentally matches. Verify Raw_Rater row 1 contains headers, not a leader's name.
