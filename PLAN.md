# Hero Forge: ASCII Arena â€” Plan

## v1 (stickman clicker) â€” replaced, kept in git history
- [x] Train mode + 10s boss fight mode with stickman heroes

## v2: ASCII arena shooter
- [x] Move project to D:\Projects\hero-forge
- [x] ASCII-rendered 3D arena: camera behind character at arena center, yaw-only mouse look (pointer lock)
- [x] Third-person back view of the character, crosshair aims with mouse Y
- [x] Click-speed duels: your clicks/s Ã— gun ROF vs enemy clicks/s decides who deals damage
- [x] Enemies shoot back, player health bar, heal between waves
- [x] Endless waves: enemies get more HP, damage and clicks/s; boss every 5th wave
- [x] Gun upgrades every 10 kills: Common â†’ Uncommon â†’ Rare â†’ Epic â†’ Legendary â†’ Mythic â†’ Cosmic â†’ endless, each with new color, ammo, effects, damage
- [x] Two versions: Black & White (only guns/bullets colored) and Full Color
- [x] Maps: Forest, Desert, Aurora (+ cycle each wave)
- [x] 4 selectable characters
- [x] Synthesized sound effects + arcade chiptune music (M to mute)
- [x] Off-screen enemy arrows + ASCII radar

## v3: real 3D + ASCII shader
- [x] three.js scene rendered through an ASCII post-process shader (glyphs sorted by ink coverage, colored per cell)
- [x] Gears-style over-the-shoulder camera, hero in lower-left, yaw-only mouse look
- [x] Forest rebuilt: tall trunks, golden canopy, god rays, fireflies, grass; desert and aurora rebuilt in 3D
- [x] 3D characters (Ranger, Ronin, Mech, Outlaw), enemies (grunt, drone, boss) with walk cycles and shatter deaths
- [x] Gun models grow per tier; tracers, sparks, explosions, chain lightning, nova rings
- [x] Contrast pass: alpha-tagged pixels; world dimmed, enemies boosted and outlined
- [x] Grand UI: Cinzel panels, segmented health, duel meter, radar, animated banners
- [x] B&W mode keeps only guns/bullets colored via the alpha tag

## v3.1: readability + champions
- [x] Champions rebuilt on a jointed rig (capsule limbs, elbows, gloves, boots) with per-character gear; all ~15% smaller, Mech much smaller
- [x] Finer glyph grid for more detail
- [x] Enemies bigger, brighter, pulsing 2-cell outline, red marker above each
- [x] Red vertical edge glows for off-screen enemies, flaring when they shoot

## v3.2
- [x] GitHub repo (public) + Vercel project asciiarena, auto-deploy on push
- [x] Gun-colored aura on the ground ahead of the hero, kept in color in B&W (own alpha tag, recolored with gun hue)
- [x] Northern lights stay colored in B&W
- [x] Cheat code: type "lasergun" to toggle 100 shots/s auto-fire
- [x] Shading pass: edge-detected contour strokes, stronger key light vs fill, smooth tone curve, calmer glyph ramp

## Next
- [ ] Playtest balance (enemy clicks/s growth vs gun ROF)
- [ ] Check frame rate on the real GPU at 1080p/1440p
