# Changelog

All notable changes to Ele-Box.

## v0.6 — 2026-06-25

### Lid logo
- **New — your own logo on the lid.** Upload an SVG (crisp vector) or a PNG (the dark part
  of the image becomes the logo), place it with its own size, position and rotation, and
  have it either engraved or as a flush 2-colour inlay in its own filament.

### Lid text
- **Fixed — the flush colour no longer disappears.** The flush inlay (text and logo) now
  comes out as a real second colour on MakerWorld and in the slicer; before, it merged into
  the lid and printed as one colour.
- **Style controls.** Bold, italic, underline and strikethrough, plus a searchable font
  picker — italic works on any font, even ones with no italic style of their own.

## v0.5 — 2026-06-24

### MakerWorld
- **Each part on its own plate.** On MakerWorld the box, lid, and (when you enable them)
  the backplate and gasket now each land on their own build plate — packed from the first
  plate with no gaps — so the customizer hands you the parts ready to print.

### Lid
- **Fixed: Inset lid + screws.** An Inset lid now sits flush on the screw posts: the posts
  shorten by one lid thickness so the lid rests level instead of proud, and the
  post-to-wall ribs stop below where the lid's lip drops in, so they no longer block it.

### Lid text
- **Flush inlay previews true.** A Flush-inlay label now shows level with the lid top and
  in colour in the All / Assembled preview — so it reads as the flush 2-colour fill it is,
  not a plain engraved recess (and the preview no longer bleeds). On MakerWorld it comes
  out on the lid's plate next to the lid, ready to give its own filament.

### Customizer
- **Slimmed.** Lip depth, fit clearance, the tongue-and-groove fit and direction, and the
  cantilever clip count moved to sensible defaults to keep the panel short.

## v0.4 — 2026-06-21

Everything in this release was 3D printed and hand-tested.

### Battery holder
- **Reworked round-cell holder.** Round cells (AAA / AA / 14500 / 18650 / C / D) now
  snap into a channel with an open centre — pinch the cell and it pops back out — and a
  standard **slide-in spring contact** sits in a slot at each end, so the holder both
  grips and **powers** the cell. This replaces the old snap-over end clips; the 9V
  holder is unchanged. Print-validated fit.

## v0.3 — 2026-06-17

Everything in this release was 3D printed and hand-tested.

### Lid closures
- **New — Tongue and groove.** A no-screws friction lid: the lip plugs into a groove in
  the rim and you pull straight up to open, with nothing that flexes and cracks. The
  groove can grow **Inner** (sides stay flush) or **Outer** (the box widens at the top
  and the lid wraps around the outside). The fit is print-validated at the default and
  tunable in 0.01 mm steps if your printer runs tight or loose.
- **New — Cantilever clips.** Press the lid down to click it shut, pull straight up to
  open; the catches hide in blind pockets in the wall (no visible holes when the wall is
  thick enough).
- **Removed Press fit, Snap lock and Removable snap lock.** The flexing ones cracked in
  PLA and the lot was fiddly; Tongue and groove and Cantilever clips replace them, with
  Screws still there for a guaranteed hold.

### Lid text
- **New — Flush inlay.** Besides engraved, the lid label can now be a separate part that
  sits level with the lid top — neither raised nor sunk — so you can print it in its own
  colour in the slicer. (The old Embossed mode is gone; it couldn't print clean on a lid
  that flips for printing.)

### Customizer
- **One "Lid" section.** All the lid options are grouped together now — about ten dials
  instead of thirty — with the rarely-touched internals moved to tidy defaults.

## v0.2 — 2026-06-14

### Standoffs
- **Per-group screw size.** Primary, secondary and individual standoffs each get their
  own self-tapping screw selector (M2 / M2.5 / M3 / M4 / M5 / M6 / 4-40 / 6-32 / 8-32 /
  Custom) that sizes that group's pilot hole. `Custom` uses the standoff hole-diameter
  field.
- **Posts auto-thicken with the screw.** The standoff outer diameter is now
  `max(base diameter, pilot + 2 × min wall)`, so a thick screw can no longer split a
  thin-walled post. Small screws keep the 7 mm base; bigger ones (e.g. M6) widen the
  post automatically. New minimum-wall setting; the diameter field is now the base /
  minimum.
- **Independent individual-standoff height.** The freely-placed (custom) standoffs have
  their own height, separate from the primary/secondary quads. Lid screw posts are
  unchanged.

## v0.1 — 2026-06-09
- Initial public release.
