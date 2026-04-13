# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a single-page static website for **Bengaluru Bootstrap Boys (BBB)**, a consulting business. The entire site lives in `index.html` — there is no build system, bundler, or backend. Open the file directly in a browser to preview changes.

## Architecture

- **`index.html`** — The entire site: inline CSS, HTML structure, and a small vanilla JS script for the rotating headline word.
- **`styleguide.json`** — Design token reference for the "Cup of Noodles" visual identity (colors, gradients, animations, component specs). Consult this before changing colors or visual styles.
- **`heropage.md`** — Copy/content reference for the consulting pitch, pricing, and bio.

## Design System

The visual identity is a "Cup of Noodles" aesthetic. All styling is inline in `index.html`. Key constraints from `styleguide.json`:

- **Color palette**: Warm reds, oranges, and golden yellows. Primary dark text uses `#8B0000` (dark red). Borders use `#8B4513` (noodle brown). Background is a radial gradient from `#FFD700` → `#DC143C`.
- **Typography**: Inter (900 weight), uppercase throughout, with multi-layer text shadows for 3D pop.
- **Animations**: Three keyframe animations — `steam` (hero background), `glow` (title text), `buttonGlow` (CTA). Keep durations as defined.
- **Layout**: `100vh` with `overflow: hidden` — everything must fit in one viewport. No scrolling.

## Contact

The WhatsApp link `https://wa.me/14156448166` appears in two places (navbar link and CTA button). Update both if the number changes.

## Frontend Design Guidelines

This skill guides creation of distinctive, production-grade frontend interfaces that avoid generic "AI slop" aesthetics.

Before coding any UI, choose a BOLD aesthetic direction — commit to one extreme: brutally minimal, maximalist, retro-futuristic, organic, luxury, brutalist, editorial, etc. Then execute it with precision.

**Typography**: Avoid Inter, Roboto, Arial, system fonts. Use distinctive, characterful choices.
**Color**: Commit to a cohesive palette. Dominant colors + sharp accents. No purple gradients on white.
**Motion**: CSS-only where possible. One well-orchestrated page load > scattered micro-interactions.
**Spatial Composition**: Asymmetry, overlap, diagonal flow, grid-breaking elements.
**Backgrounds**: Gradient meshes, noise textures, geometric patterns — not flat solid colors.

NEVER produce generic AI aesthetics. Every design should be unmistakably different from the last.
