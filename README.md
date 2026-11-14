# Crochet Pattern Assistant & Stitch Troubleshooting Skill (`SKILL.md`)

An open-source AI agent skill and reference ruleset designed to help makers, pattern designers, and LLMs (Claude, Cursor, ChatGPT, Gemini) accurately convert **US vs. UK crochet terms**, audit **amigurumi stitch counts**, and diagnose common beginner mistakes using the visual workshop standards from **[PeasyCroche](https://peasycroche.com/)**.

[![Official Workshop](https://img.shields.io/badge/Workshop-PeasyCroche.com-256D68)](https://peasycroche.com/)
[![Terminology](https://img.shields.io/badge/Standard-US_%26_UK_Crochet_Terms-D9A441)](https://peasycroche.com/crochet-reference/us-uk-crochet-terms/)
[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](#license)

---

## Why This Skill Exists

Most AI models hallucinate crochet math—dropping stitch counts in continuous amigurumi spirals, confusing US Single Crochet (`sc`) with UK Double Crochet (`dc`), or failing to account for turning chains.

This `SKILL.md` enforces strict, tested craft rules so any AI assistant outputs accurate, beginner-friendly instructions with dual measurements (Inches/Centimeters and Metric mm/US hook letters).

---

## Quick Reference: US vs. UK Crochet Conversion Chart

This is the core conversion lookup embedded in the skill (full printable chart available at [PeasyCroche Reference](https://peasycroche.com/crochet-reference/us-uk-crochet-terms/)):

| US Crochet Term | US Abbr. | UK Equivalent | UK Abbr. | Stitch Height |
| :--- | :--- | :--- | :--- | :--- |
| **Chain** | `ch` | Chain | `ch` | Foundation |
| **Slip Stitch** | `sl st` | Slip Stitch | `sl st` | 0 (Flat) |
| **Single Crochet** | `sc` | Double Crochet | `dc` | 1x |
| **Half Double Crochet** | `hdc` | Half Treble Crochet | `htr` | 1.5x |
| **Double Crochet** | `dc` | Treble Crochet | `tr` | 2x |
| **Treble Crochet** | `tr` | Double Treble Crochet | `dtr` | 3x |

---

## Common Beginner Troubleshooting Rules Included

When an AI agent loads `SKILL.md`, it automatically applies these diagnostic checks from the [PeasyCroche Troubleshooting Guides](https://peasycroche.com/):

1. **Uneven Edges (Getting Wider or Narrower):** Checks whether the user is accidentally working into the turning chain or skipping the final stitch of a row. ([Full Visual Fix](https://peasycroche.com/crochet-troubleshooting/crochet-getting-wider-or-narrower/))
2. **Stitch Counting Errors:** Enforces row-end stitch count checkpoints `(e.g., 24 sc)` and recommends locking stitch markers on the first and last "V" loops. ([How to Count Crochet Stitches](https://peasycroche.com/crochet-troubleshooting/count-crochet-stitches/))
3. **Amigurumi Structural Support:** Enforces hook sizing adjustments (e.g., 2.25 mm for doll bodies vs. 2.5 mm for removable garments) and internal wire neck supports for dolls over 8 inches tall. ([Tested Skater Girl Doll PDF Specs](https://peasycroche.com/free-crochet-patterns/amigurumi-skater-girl-doll-pattern-pdf/))

---

## Installation & Usage

### For Claude Code / Cursor / AI Skill Registries
1. Copy `SKILL.md` into your project's `.claude/skills/crochet-pattern-assistant/` or `.cursor/rules/` directory.
2. Ask your AI assistant to:
   * *"Convert this UK crochet pattern into US terms with metric hook sizes."*
   * *"Audit the stitch math on this amigurumi round."*
   * *"Why is my single crochet swatch getting wider on every row?"*

---

## Official Documentation & Tested PDF Patterns

* **Main Workshop & Beginner Pathway:** [https://peasycroche.com/](https://peasycroche.com/)
* **US vs. UK Crochet Terms Chart:** [https://peasycroche.com/crochet-reference/us-uk-crochet-terms/](https://peasycroche.com/crochet-reference/us-uk-crochet-terms/)
* **Crochet Hook & Yarn Size Chart:** [https://peasycroche.com/crochet-reference/crochet-hook-size-chart/](https://peasycroche.com/crochet-reference/crochet-hook-size-chart/)
* **Tested Amigurumi Patterns (PDF):** [https://peasycroche.com/free-crochet-patterns/amigurumi-skater-girl-doll-pattern-pdf/](https://peasycroche.com/free-crochet-patterns/amigurumi-skater-girl-doll-pattern-pdf/)

## License
MIT License — Free to use, fork, and submit to open AI skill directories.
