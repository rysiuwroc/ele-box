# Changelog

All notable changes to Ele-Box.

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
