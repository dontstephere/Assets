Nova Blizzard Stone - Layered Panel System v1
===========================================

This pack fixes the 'every texture looks like the same square tile' problem by splitting
the look into TWO layers, like Blizzard UI:

A) Shared tiled material:
   Shared/stone_tile_256.tga  (repeat/tiling recommended)

B) Panel-shaped overlays:
   NeutralOverlays/<Panel>Overlay_WxH.tga  (vignette/corner dirt/lighting)
   Classes/<Class>/Overlays/<Panel>Overlay_WxH.tga (same overlay, class-tinted)

If you CANNOT tile in your renderer, use FullBaked textures:
   NeutralFullBaked/<Panel>_WxH.tga
   Classes/<Class>/FullBaked/<Panel>_WxH.tga

Recommended render order (best quality):
  1) Draw tiled base (stone_tile_256) with white tint & low alpha (~0.06-0.10)
     - If tiling supported: SetHorizTile/SetVertTile and set TexCoord based on frame size.
  2) Draw overlay for that panel (class overlay if using option 2) with white tint (alpha already baked).
  3) Draw borders/toggles/highlights with ACCENT_PRIMARY.

