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
