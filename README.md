# Razer Wolverine V3 TE Controller Overlay

<p align="center">
  <img src="docs/preview.png" alt="Razer Wolverine V3 TE controller overlay preview" width="720">
</p>

<p align="center">
  A custom SVG controller-overlay skin with a clean topographic look, dedicated pressed states, trigger/bumpers, D-pad feedback, stick clicks, and alternate button-state assets.
</p>

## ✨ Features

- Custom controller shell / base artwork
- SVG assets for crisp scaling at any stream resolution
- Individual **A / B / X / Y** normal and pressed states
- **D-pad** pressed states for all four directions
- **LB / RB / LT / RT** pressed states
- Combined **LT + RT** state
- Stick and stick-click states
- Menu / switcher states
- Disconnected-state artwork
- Alternate `M1` / `M2` state assets
- Stream-friendly transparent SVG workflow

## 📦 Repository structure

The runtime SVG files intentionally stay in the repository root. Many controller-overlay setups reference these filenames directly, so moving them into folders can break the skin.

```text
Razer-Wolverine-V3-TE-Overlay/
├── README.md
├── CHANGELOG.md
├── .gitignore
├── docs/
│   ├── preview.png
│   ├── ASSET_MAP.md
│   └── CUSTOMIZATION.md
│
├── base.svg
├── base2-0.svg
├── base2-0-b-m2.svg
├── base2-0-b-m2-off.svg
├── base2-0-y-m1.svg
├── base2-0-y-m1-off.svg
│
├── a.svg
├── a-pressed.svg
├── b.svg
├── b-pressed.svg
├── x.svg
├── x-pressed.svg
├── y.svg
├── y-pressed.svg
│
├── up-pressed.svg
├── down-pressed.svg
├── left-pressed.svg
├── right-pressed.svg
│
├── lb-pressed.svg
├── rb-pressed.svg
├── lt-pressed.svg
├── rt-pressed.svg
├── lt-and-rt-pressed.svg
│
├── stick.svg
├── stick-pressed.svg
├── menu-pressed.svg
├── switcher-pressed.svg
└── disconnected.svg
```

## 🚀 Using the skin

1. Download or clone this repository.
2. Keep the runtime SVG filenames unchanged unless you also update the overlay configuration that points to them.
3. Use the SVGs in the same controller-overlay setup you currently use for your stream/browser source.
4. Resize the browser/source in OBS as needed. Because the artwork is SVG, it remains sharp when scaled.

> **Tip:** If you customize a file, make a backup first. The pressed-state files need to line up pixel-perfectly with the base artwork.

## 🗺️ Asset reference

A full file-by-file explanation is available in [`docs/ASSET_MAP.md`](docs/ASSET_MAP.md).

For safe editing tips, see [`docs/CUSTOMIZATION.md`](docs/CUSTOMIZATION.md).

## 🛠️ Editing

For visual edits, an SVG editor such as **Inkscape** is ideal. Canva can import many SVGs, but complex masks, clipping paths, filters, or grouped layers may not round-trip perfectly.

When changing the controller design:

- Preserve the existing canvas size / `viewBox`.
- Keep interactive pieces aligned with the base image.
- Avoid renaming IDs if your overlay code targets them.
- Export as SVG, not raster PNG, for runtime assets.

## 🎮 Design notes

This skin is built around a dark controller body with a topographic-inspired visual treatment and separate state artwork so inputs can light up cleanly without redrawing the whole controller every frame.

## 📸 Preview

The preview above is rendered directly from `base2-0.svg`, so the repository always contains a quick visual reference for the current base design.

## 🧩 Planned / optional improvements

- Add an animated live demo GIF
- Add a one-click hosted demo page
- Add alternate colorways
- Add a dedicated source/template folder for editable master artwork
- Add versioned releases for stable skin packs

## Credits

Designed and customized by **AresDza**.

If you build on this project, credit is appreciated.
