# Nucleon — Cosmetic Assets

Public assets for the **Nucleon** Minecraft client, served via [jsDelivr](https://www.jsdelivr.com/).
Original, procedurally-generated (not derived from any copyrighted cape).

## Capes

`capes/<name>_sheet.png` — a vertical sprite sheet of **60 frames** (each 512×256, indexed PNG with
transparency) in Minecraft's cape + elytra texture layout. The client downloads & disk-caches the
sheet, slices it into frames, and animates them.

Served at:

```
https://cdn.jsdelivr.net/gh/OsmiumGoated/Nucleon-assets@main/capes/<name>_sheet.png
```

Current capes: **aura**, **dragon**, **tempest**.

## Updating / adding a cape

1. Replace (or add) a `*_sheet.png` here and push.
2. jsDelivr caches `@main` for a while — purge instantly at
   `https://purge.jsdelivr.net/gh/OsmiumGoated/Nucleon-assets@main/capes/<name>_sheet.png`.
3. Players also disk-cache; clearing `.minecraft/nucleon/capecache/` forces a re-fetch.

(Adding a brand-new cape also needs a matching entry in the client's `CapeStyle` enum.)

Generated from the Nucleon `capes/` workspace (`generate/capelib.py`).
