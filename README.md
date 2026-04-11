![MFT Workbench Banner](./banner.png)

# MFT Workbench Project

This repository is a **woodworking project**, not a software project.

It contains the build drawings and cut list for an MFT-style workbench system made from sheet goods and framing stock.

## What’s in this repo

- `20260220-workbench.svg` — source drawing (Inkscape)
- `20260220-workbench.png` — PNG render exported from the SVG
- `20260220-workbench.pdf` — plan export
- `20260220-workbench-cutlist.pdf` — printable cut list
- `banner.svg` / `banner.png` — GPT-generated README banner

## Drawing summary (from the SVG)

The SVG appears to include:

- Two table configurations: **Table A** and **Table B**
- Labeled part families for cabinets, table structure, drawers, and trolley components
- Dimension callouts in millimeters (e.g. 1800mm, 1200mm, 800mm, 700mm, 600mm, 400mm, 200mm, 100mm, 90mm)
- Material thickness callouts including **17mm** (sheet stock) and **8.5mm** (likely panel/back/bottom detail)

A visual render of the plan:

![Workbench Plan](./20260220-workbench.png)

## Extracted cut list text (as labeled in the SVG)

> Verify all measurements against the original SVG/PDF before cutting.

### Table A / Cabinet A

- `A.CabinetBack` — qty 3 — `17 x 700 x 400`
- `A.CabinetSide` — qty 6 — `17 x 700 x 600`
- `A.CabinetBottom` — qty 3 — `17 x 600 x 400`
- `A.TableBottom` — qty 1 — `17 x 1800 x 600`
- `A.TableSide` — qty 2 — `17 x 1800 x 200`
- `A.DrawerFace` — qty 20 — `17 x 400 x 140`
- `A.DrawerSides` — qty 40 — `17 x 550 x 110`
- `A.DrawerBase` — qty 20 — `17 x 480 x 332`
- `A.DrawBack` / `A.DrawerBack` — qty 20 — `17 x 332 x 110`
- `A.TableTop` — qty 1 — `17 x 1800 x 600`

### Shared / Support parts

- `TableEnd` — qty 7 — `17 x 566 x 200`
- `TableSupports` — qty 6 — `17 x 800 x 100`
- `TableSupportsTrolly` — qty 2 — `17 x 612 x 100`
- `TableFeet` — qty 8 — `90 x 45 x 100`

### Table B / Cabinet B / Trolley B

- `B.CabinetBack` — qty 1 — `17 x 1200 x 700`
- `B.CabinetSide` — qty 4 — `17 x 600 x 700`
- `B.CabinetBottom` — qty 3 — `17 x 400 x 600`
- `B.TableBottom` — qty 1 — `17 x 1200 x 600`
- `B.TableSide` — qty 2 — `17 x 1200 x 200`
- `B.TrollyBottom` — qty 1 — `17 x 500 x 600`
- `B.TrollyBackFront` — qty 2 — `17 x 500 x 512`
- `B.TrollySides` — qty 2 — `17 x 500 x 600`
- `B.TableTop` — qty 1 — `17 x 1200 x 600`
- `B.TrollyTop` — qty 1 — `17 x 600 x 600`

## Export notes

The original SVG canvas is very large (`16000mm x 4000mm`).
For practical viewing, the PNG in this repo was exported at a fixed width of `3200px`.

Example export command:

```bash
inkscape 20260220-workbench.svg \
  --export-type=png \
  --export-filename=20260220-workbench.png \
  --export-width=3200
```

---

If you want, I can also add:

1. a **material yield plan** (how many sheets/boards needed),
2. a **build sequence** checklist (assembly order), and
3. a **hardware/BOM** section (slides, screws, inserts, etc.).
