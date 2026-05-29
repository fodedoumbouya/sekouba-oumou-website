# Oumou & Sekouba — Wedding Website Design Spec

## Overview
Single-page wedding invitation website for the two-day celebration of Oumou & Sekouba.
Language: French. Style: Traditional Elegance (ivory, gold, serif).

## Aesthetic
- **Palette:** Ivory `#F5EDD8`, Gold `#C49848`, Dark Brown `#3D2B0D`
- **Typography:** Playfair Display (headings, italic) + Inter (body)
- **Mood:** Warm, romantic, West African cultural celebration
- **Motion:** Gentle falling flower petals (canvas), subtle GSAP scroll reveals
- **Music:** Ambient background music with mute/unmute toggle

## Sections (one-page scroll)
1. **Hero** — couple illustration + names + dates + "Avec leurs familles" + petal overlay
2. **Jeudi 25 Juin — Mariage Religieux** — gold timeline, bg image blend
3. **Samedi 27 Juin — Mariage Civil** — gold timeline (8 items), bg image blend
4. **Les Lieux** — two venue cards with Google Maps links
5. **RSVP** — form: name, guest count, attendance, day(s), message
6. **Footer** — names + date + "Avec leurs familles"

## Background Images
Each section has a low-opacity (8–12%) floral/botanical image via `::before` pseudo-element with `mix-blend-mode: multiply`, so it blends naturally into the ivory background.

## Falling Petals
Canvas overlay (fixed, full viewport, `pointer-events: none`). ~60 petals at varied sizes, speeds, and gold/ivory colors with sine-wave drift.

## Music
HTML5 `<audio loop>` with a sticky mute/unmute button. User drops `music.mp3` into the project folder.

## Content
- **Day 1:** 25 Jun 2026 · 14h00–19h00 · 1 rue des Jonquilles, 91140 Villebon-sur-Yvette
- **Day 2:** 27 Jun 2026 · 15h00–3h30 · Place Gérard-Nevers, 91140 Villebon-sur-Yvette
- **Couple illustration:** `couple.png` (extracted from invitation video)
