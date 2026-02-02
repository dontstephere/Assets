Nova Blizzard-Style Panel Material Pack
======================================

Goal: subtle Blizzard-like panel material (neutral, not class-colored).
Use the 'Sized' textures if your renderer stretches textures.
Use the 'Tileable' textures if you implement tiling/repeat.

Recommended draw order:
1) Base fill: BG_PANEL / BG_NAV (neutral dark)
2) Overlay material: use white tint with low alpha

Suggested alpha (8-bit):
- Large panels (ContentPanel / BorderFrame): 10-14 (4-6%)
- Small controls (buttons/checkbox): 8-12 (3-5%)

Important: do NOT tint the material with class colors.
Apply class color only to borders, toggles, highlights.
