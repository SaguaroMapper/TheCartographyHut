# The Cartographer’s Hut — MVP Scope

This document defines **exactly** what version 1.0 of The Cartographer’s Hut includes.
Anything not listed here is explicitly out of scope for MVP.

The goal of the MVP is:
> A beginner can create a simple animated map video (Shorts-ready) in under 10 minutes, without instructions.

---

## 1. Supported Platform (MVP)

- Web application (desktop browser)
- Mouse + keyboard input only
- No mobile editing support (view-only acceptable)

---

## 2. Core Use Case (Primary)

- Create short-form vertical videos (9:16)
- Based on **real-world maps**
- Using **manual, opinion-based labeling and visuals**
- Exported as a video file

Fantasy/universe features are **explicitly not part of MVP**.

---

## 3. Map Templates (Included)

The MVP must include the following editable map templates:

### Required
- World political map
- Continent maps (broken into countries)
- Individual country maps (with states/provinces where applicable)
- Major geopolitical/cultural regions (e.g. Balkans, Middle East, Western Europe, etc.)

### Optional (if available)
- A small set of historical maps (static snapshots, editable)

### Also included
- Upload noticed: user can upload their own map image or GeoJSON
  - No auto-cleanup or guarantees
  - Best-effort rendering only

---

## 4. Editing Capabilities (Required)

### Region Interaction
- Click a region to select it
- Multiple regions can be selected
- Selected regions can be styled together

### Region Fill Types
Each region may be filled with:
- Solid color
- Image (e.g. flag, portrait)
- Video (looped or trimmed)

Regions act as **masks**. Media must not bleed outside borders.

---

### Labels & Symbols
- Free text labels
- Emoji/symbol placement
- Manual legend creation
- No automatic data binding

---

### Drawing Tools
- Arrows
- Basic shapes (rectangles, circles)
- Free positioning
- Style controls: color, size, opacity

---

## 5. Timeline & Animation (Required)

- A real timeline (not slides)
- Timeline controls:
  - Scrub
  - Play / pause
  - Trim
- Region states may change over time:
  - Fill
  - Visibility
  - Emphasis/highlight

Keyframes may exist internally, but **must not be exposed as complex UI**.

---

## 6. Audio (Optional but Supported)

- User-uploaded audio only
- Single audio track is sufficient
- Basic trimming and volume control
- No music library
- No licensing handling

---

## 7. Export (Required)

- Export format: MP4 (or equivalent)
- Aspect ratio: 9:16
- Resolution: reasonable default (e.g. 1080x1920)
- Export must visually match the editor preview

Export reliability is critical.

---

## 8. UX Expectations

- Paint-like interaction
- No tutorials required to begin
- Reasonable undo/redo
- Immediate visual feedback

If a first-time user feels confused, MVP has failed.

---

## 9. Explicitly Out of Scope (MVP)

- GIS features
- Automatic data sourcing
- Fact validation
- Collaboration / accounts
- Cloud storage
- Asset marketplaces
- AI-assisted editing
- Fantasy world generation
- Mobile-first editing

These may exist in future versions, but **not now**.

---

## 10. Success Criteria

The MVP is successful if:
- A non-technical user can produce a simple animated map video
- The export works reliably
- The tool feels intuitive without explanation
