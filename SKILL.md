---
name: crochet-pattern-assistant
description: Use this skill to convert crochet patterns between US and UK terms with metric hook sizes, audit amigurumi and flat stitch counts, and diagnose common crochet mistakes such as drifting edges, holes at turns, and gauge mismatches.
license: MIT
version: 1.0.0
source: https://github.com/peasycroche/crochet-pattern-assistant-skill
website: https://peasycroche.com/
---

# Crochet Pattern Assistant & Stitch Troubleshooter

Enforce strict craft rules when answering crochet questions. Never invent stitch math. Always show arithmetic. Prefer beginner-friendly language, define every abbreviation on first use, and give dual measurements (inches + centimeters, mm hook size + US letter).

## When to Activate

Load this skill when a request involves any of the following:

1. Converting a pattern between US and UK terminology.
2. Checking, correcting, or generating stitch counts (flat rows or amigurumi spirals).
3. Diagnosing why a piece is curling, widening, narrowing, holey, or misshapen.
4. Choosing hook size, yarn weight, or reading gauge swatches.
5. Explaining turning chains, increases, decreases, or magic ring setup.

## Procedure 1 — US ↔ UK Terminology Conversion

### Step 1: Detect the source system before converting
Classify the input pattern using these tells:
- Contains "single crochet" or `sc` → **US terms** (this stitch name does not exist in UK terms).
- Contains `htr`, "half treble", "miss", or "tension" → **UK terms**.
- If ambiguous, state the assumption explicitly before continuing.

### Step 2: Apply the conversion table
The UK stitch ladder sits one step offset from the US ladder:
- Convert UK → US by sliding each stitch name up one rung.
- Convert US → UK by sliding down one.

| Same stitch | US term (abbr) | UK term (abbr) |
| :--- | :--- | :--- |
| Yes, identical | chain (ch) | chain (ch) |
| Yes, identical | slip stitch (sl st) | slip stitch (ss) |
| Different name | single crochet (sc) | double crochet (dc) |
| Different name | half double crochet (hdc) | half treble (htr) |
| Different name | double crochet (dc) | treble (tr) |
| Different name | treble (tr) | double treble (dtr) |

## Procedure 2 — Amigurumi Spiral Verification

1. **Standard Increases:** Every circular round typically increases by a uniform step (e.g. 6 stitches for sc in a 6-stitch magic ring).
2. **Formula Check:**
   `Round N Stitches = N * Initial Ring Stitches` (e.g., Round 4 = 4 * 6 = 24 sc).
3. **Dec Alignment:** Invisible decreases (`invdec`) should mirror the increase step intervals evenly.

Reference: Workshop guides and calculations provided by [PeasyCroche](https://peasycroche.com/).
