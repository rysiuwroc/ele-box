# Ele-Box

**From bare-bones to fully loaded.** You choose every feature — and the size.

**v0.2 · 2026-06-14** — see what's new in the [changelog](CHANGELOG.md).

> 🐛 **Found a bug? Want a feature? Have a question?**
> File it on the **[Issues page →](https://github.com/rysiuwroc/ele-box/issues)** —
> pick a type (bug / feature / question) and it gets sorted automatically. That's the
> one place for everything.

Ele-Box is a fully parametric enclosure for 3D-printable electronics and project
builds: a box plus a matching lid, with an optional gasket and backplate. Set your
inside dimensions, toggle the features your build actually needs — screw posts,
ports, vents, standoffs, glands, snaps, seals — and you get a print-ready box laid
out flat on the bed. The default is 160 × 100 × 40 mm inside, with 3 mm walls, floor
and lid and a 5 mm corner radius. Change any of it. Made for Bambu Lab.

## What you can generate

Choose what to print:

- **All** — base + lid (and backplate, if enabled), laid out side by side
- **Base only** — the box body
- **Lid only** — the lid
- **Gasket only** — a flat sealing ring to print in TPU
- **Backplate only** — an internal plate drilled to match your standoffs

And how it comes out:

- **Layout:** Print (flat on the bed, lid pre-flipped) or Assembled (stacked as it
  fits together, for a sanity check).
- **Split:** halve an oversized model — Length A/B or Width A/B — for a small bed.
  It's a plain straight cut, so glue or dowel the seam yourself.
- **Quality:** Low, Normal, Fine or Very fine curve smoothness — drop it while
  experimenting, crank it for the final.

## Box body

- Inside length / width 20–300 mm, inside height 10–180 mm.
- Wall, floor and lid thickness 1.2–8 mm each.
- Outer corner radius 0–30 mm (0 = sharp corners).
- Fit clearance between base and lid, plus a plug-in lip with tunable depth and wall
  thickness.

## Lid mounting

Six ways to close it — Screws, Press fit, Snap lock, Removable snap lock, Glue, or a
Plain plate — with the lid shaped as a **Cap** (sits over the rim) or **Inset**
(drops flush into the opening).

- **Screws** — base posts sized for M2, M2.5, M3, M4, M5, M6, 4-40, 6-32, 8-32 or a
  custom size. Head recess socket/pan, flat countersunk, or none. Set post diameter,
  inset and the rib that blends each post into the wall.
- **Snap lock** latches all four sides; **Removable snap lock** latches only the
  length sides so the lid pops back open. Tune catch height, reach, width and
  position below the rim.
- **Press fit** — grip ribs on none / length / width / four sides. Net grip is rib
  depth minus fit clearance (about 0.25 mm per side by default): deepen for tighter,
  raise clearance for looser.
- **Glue / Plain plate** for the simplest builds.

## Openings

- **Round and rectangle holes** in the lid top or any side wall, as parametric rows
  with rounded corners — set count, size, offset, spacing and axis for connectors,
  switches and displays.
- **Vent grids** — slots or round holes with independent row and column spacing: up
  to 12 rows × 20 columns on the lid, up to 10 rows × 20 columns on a side wall.
- **Panel connectors** — up to 4 cutouts from named presets that set the exact
  opening: USB-A, USB-C, Micro-USB, Mini-USB, RJ45 Ethernet, HDMI-A, DC barrel jack,
  Audio 3.5 mm, SMA antenna, DB9 serial. Each picks its wall, height and offset, with
  an oversize option to clear a whole plug body when a port sits back from the wall.
- **Cable glands** — PG7 / PG9 / PG11 / PG13.5 / M12 / M16 / M20 or custom, 1–6 per
  wall, with an optional inner boss so the gland nut has material to bite into.

## Board fit and ports that line up

This is where Ele-Box earns its keep. Two things have to be right: the hole sits
where the port is, and the port actually reaches the wall.

- **Standoffs** — a primary quad set to your board's hole pattern, an optional second
  quad, and up to 4 individually placed posts. Out-of-bounds standoffs are trimmed to
  the interior automatically, so nothing prints floating.
- **Board anchor** — define the board outline and park its port edge a small gap from
  a chosen wall, then reference your connectors to the board so the cutouts auto-align
  to the real ports.
- **Preview ghost** — a translucent board outline you can switch on to line things up
  (preview only, never printed).
- **Backplate** — a separate internal plate drilled to match every enabled standoff
  group, with its own wall gap, thickness and corner rounding.

## Onboard hardware

- **Battery holder** — snap-in cradles that self-size to AAA, AA, 14500, 18650, C or
  D cells, 1–4 across. End clips grip just past center; a 9V block gets an open-top
  well for the snap clip and leads.
- **Display window** — a rounded screen cutout with an optional inner ledge so an
  OLED/LCD drops in from inside and rests on the step.
- **LED indicators** — 3 mm / 5 mm / custom holes in a row, 1–8 across, with an
  optional underside collar to align and grip each LED.

## Mounting and finishing

- **Base mounting** — side tabs, corner ears, a full flange, or floor holes; on the
  length, width or all sides; one centered hole or two near the corners. Fixings can
  be round, slot or keyhole, in compact / normal / large sizes.
- **Waterproof gasket** — shrinks the lip and cuts a sealing channel with a retaining
  ridge. Print the flat gasket ring in TPU (PLA/PETG stays too rigid to seal), or use
  it as a cutting template for rubber or foam.
- **Rubber feet** — shallow recesses in the four bottom corners for stick-on feet.
- **Lid text** — an embossed or engraved label with your own string, font, size,
  position and rotation.

## Make it your size

Every dimension and every feature is a setting. Punch in your inside length, width
and height, pick a lid style, toggle the features you need, and you get a print-ready
box — anywhere from a 20 mm trinket case up to a 300 mm enclosure. No remodeling, no
guesswork.

## Printing

- **No supports.** The base prints open-side up and the lid prints top-down
  (pre-flipped for you in the print layout). Standoffs, battery cradles, LED collars
  and the display ledge all grow up from a surface, so there's nothing to bridge.
- The one overhang is the optional inner boss on round ports — it's off by default
  and short enough to bridge, but add a chamfer if your printer struggles with it.
- Size the box for what goes in it: cradles and ports land where you ask without
  enlarging the box, so check that your inside dimensions clear the cell length and
  connector height.

From a USB breakout to an 18650 power bank, it's one parametric box. Pick the parts,
set the size, print.

---

Free for everybody, for personal, non-commercial use — print all you like, just
don't sell it. Not monetizable, not for resale. Closed-source design; the source
files are not distributed.
