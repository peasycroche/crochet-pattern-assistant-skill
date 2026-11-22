# Crochet Pattern Assistant & Stitch Troubleshooter

An open-source AI agent skill, reference toolkit, and structured ruleset for makers, pattern designers, and LLMs (Claude, Cursor, ChatGPT, Gemini, Copilot).

Developed by [PeasyCroche](https://peasycroche.com/), this toolkit standardizes US versus UK crochet terminology conversions, amigurumi math verification, and systematic troubleshooting for common tension and turning errors.

---

## 🧶 Features

- **Bidirectional Terminology Conversion:** Seamlessly convert patterns between US and UK stitch terms with metric hook equivalents.
- **Amigurumi Arithmetic Auditing:** Verify stitch counts per round across spiral increases, decreases, and flat row expansions.
- **Error Diagnosis & Troubleshooting:** Pinpoint reasons for edge drift, curling fabric, holes at turning chains, and tension gauge mismatches.
- **Agent & LLM Compatible:** Ready-to-load `SKILL.md` ruleset engineered for Claude Code, Cursor, Copilot, and custom agent workflows.

---

## 📖 Conversion Quick Reference

| Stitch | US Term (Abbr) | UK Term (Abbr) | Height |
| :--- | :--- | :--- | :--- |
| Chain | chain (`ch`) | chain (`ch`) | Base rung |
| Slip Stitch | slip stitch (`sl st`) | slip stitch (`ss`) | Joining |
| Single / Double | single crochet (`sc`) | double crochet (`dc`) | 1 ch height |
| Half Double / Half Treble | half double crochet (`hdc`) | half treble (`htr`) | 2 ch height |
| Double / Treble | double crochet (`dc`) | treble (`tr`) | 3 ch height |
| Treble / Double Treble | treble (`tr`) | double treble (`dtr`) | 4 ch height |

---

## 🚀 Installation & Usage

### 1. In Claude Code / Cursor / AI IDEs
Place [`SKILL.md`](SKILL.md) in your project's `.claude/skills/` or prompt instructions directory:
```bash
# Clone repository
git clone https://github.com/peasycroche/crochet-pattern-assistant-skill.git
```

### 2. Live Craft Reference
Visit [peasycroche.com](https://peasycroche.com/) for visual video walkthroughs, stitch count calculators, and free designer patterns.

---

## 📜 License
MIT License © 2026 [PeasyCroche](https://peasycroche.com/).
