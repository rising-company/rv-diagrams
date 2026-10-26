# RV Diagrams

Interactive 3D diagrams for RV electrical systems, built as self-contained HTML files with no build step required.

## Diagrams

### `battery-box.html` — Battery Box Structure

An interactive 3D visualization of an RV battery box showing the physical layout and wiring of a dual LiFePO4 battery bank.

**What it shows:**

- Wood frame (edge-beam cube construction with 4 corner posts, bottom rails, top rails)
- Bottom EVA foam isolation pad
- 2x 100Ah 12V LiFePO4 batteries wired in parallel
- Brass terminals on each battery (positive and negative)
- Top foam buffer pads + top retention beam (2x4 lumber)
- Positive and negative bus cables linking the parallel bank
- Output (+) and output (−) leads exiting through the side walls

**Controls:**

| Input | Action |
|-------|--------|
| Drag | Rotate the view |
| Scroll / Pinch | Zoom in/out |
| Hover over a part | Show component name, material, and description |

The scene auto-rotates until you interact with it.

**System specs shown:**

| Spec | Value |
|------|-------|
| System voltage | 12V / 24V |
| Battery type | LiFePO4 Lithium |
| Battery count | 2x 100Ah (parallel) |
| Frame material | 2x4 lumber |
| Padding | Closed-cell EVA foam |
| Bus cable | 2 AWG |
| Output leads | 4 AWG |

### `cabin.html` — Airstream Safari 25′ Cabin

An interactive walkthrough of a 2003 Airstream Safari 25′ (Model 25A floorplan, modified
with a king-bed conversion at the rear and a U-shaped front dinette).

**What it shows:**

- Curved aluminium shell with windows, tandem axle, A-frame tongue, propane tanks and rooftop A/C
- Entry door that swings open, and a camera move that steps you inside
- First-person cabin: galley, fridge column, corner end table, mid-bath (shower, lavatory, toilet), wardrobes, U-dinette and king bed
- Bathroom door (swings out into the aisle) and a roll-up shower door
- Curb-side awning that extends and retracts; reflective riveted aluminium shell with rock guard and stone guard
- Roof cutaway view of the whole layout from outside

**Controls:**

| Where | Input | Action |
|-------|-------|--------|
| Outside | Drag / Scroll / Pinch | Orbit and zoom |
| Outside | Click entry door | Open it, click again to step inside |
| Inside | Drag | Look around |
| Inside | WASD / Arrow keys | Walk |
| Inside | Click floor | Walk there (routes through the bath doorway) |
| Inside | Click a door | Open or close it; walking out the entry door returns outside |

Buttons in the navigation panel do the same things and jump between rooms.

**Dimensions are approximate.** Every size lives in the `L` layout block and the
`OPENINGS` list at the top of the script, in inches, measured from the centre of the
cabin floor. They were scaled from the factory floorplan (calibrated on its labelled
32″×78″ beds and 31⅝″×42″ dinette), so swap in tape measurements as you take them.

## Usage

Open any HTML file directly in a browser — no server or dependencies needed beyond an internet connection for Google Fonts and the Three.js CDN.

```bash
open battery-box.html
```

## Tech Stack

- [Three.js r128](https://threejs.org/) — 3D rendering via WebGL
- Vanilla HTML/CSS/JS — zero build tooling
- Google Fonts: Share Tech Mono, Rajdhani

## License

See [LICENSE](LICENSE).
