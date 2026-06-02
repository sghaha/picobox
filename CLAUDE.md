# CLAUDE.md — picobox

## Project Overview

**picobox** is a custom arcade-style all-button (hitbox-layout) game controller built on a Raspberry Pi Pico (Micro Plus). This repository is a **documentation-only project** — it contains no firmware, source code, or build system. All content is in Korean.

## Repository Contents

| File | Description |
|---|---|
| `README.md` | Project landing page with embedded images |
| `기본사용법.png` | "Basic Usage" guide — button combinations and RGB LED control |
| `핀배치.png` | "Pin Layout" diagram — physical button numbering on the controller face |

## Hardware

The controller is a hitbox-style layout with **19 numbered buttons**:

- **Directional inputs**: buttons 1–5 (left-side cluster)
- **Action buttons**: buttons 6–10, 14–17 (right-side, mapped to face/shoulder buttons)
- **System buttons**: button 11 = START, button 12 = BACK, button 13 = HOME
- **Extra buttons**: 18, 19 (top-left auxiliary)
- **Face button mapping**: A/× (5), B/○ (6), X/□ (7), Y/△ (8), RB/R1, RT/R2, LB/L1, LT/L2, and additional

The PCB branding reads **PiCO BOX MICRO PLUS**, indicating the Raspberry Pi Pico as the MCU.

## Key Features (documented in 기본사용법.png)

- **Combo shortcuts** — e.g. BACK + START = HOME/OK
- **RGB LED control** — BACK + START + directional/action button combinations cycle colors and effects
- **SOCD (Simultaneous Opposing Cardinal Directions)** — configurable SOCD cleaning mode for fighting-game compliance
- **5-button mode** — alternate button configuration accessible via a key combo

## Working in This Repository

### This is a docs-only repo
There is no firmware, no build pipeline, no test suite, and no package manager. All contributions are either:
- **Image updates** — replace/add `.png` files documenting hardware layout or usage
- **README updates** — edit `README.md` in Markdown

### Conventions
- Images use Korean filenames matching their subject (e.g. `기본사용법.png` = "basic usage")
- The README only embeds images; descriptive text lives inside the images themselves
- Commits have been simple `"Update README.md"` messages — match this style for minor doc tweaks

### No build/test steps required
There is nothing to install, compile, or test. Editing Markdown and PNG files is the full workflow.

## AI Assistant Notes

- Do **not** attempt to run build commands — none exist
- Do **not** create `package.json`, `requirements.txt`, or any build scaffolding unless explicitly requested
- When updating documentation, prefer editing existing files over creating new ones
- If firmware source code is added in future, update this file to document the build system, flashing instructions, and test approach
- The primary audience and documentation language is **Korean**; respect that in any new content
