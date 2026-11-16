# Meta Quest 2 Benchmark: Minecraft Java via Horizon VR

Performance test of Minecraft Java Edition running through Horizon VR on a Meta Quest 2 in standalone mode.

## Setup

| Item | Value |
|---|---|
| Headset | Meta Quest 2 (standalone) |
| OS | Latest version |
| VR app | Horizon VR (unofficial VR port of the Horizon client) |
| Game | Minecraft Java Edition 26.3 |
| Renderer | Vulkan |
| Refresh rate | 72 Hz |
| Max framerate | 120 FPS |
| Anti-aliasing | Off |
| Render distance | 16 chunks |
| Simulation distance | 6 chunks |
| LOD | Enabled |
| Chunk fade | 0.75 s |
| VSync | On |
| Culling | Entity, cave and particle culling on |

## Results

| Criterion | Score |
|---|---|
| Performance | 8/10 |
| Image quality | 5/10 |
| Stability | 7/10 |

- **Performance**: most scenes run near or above 72 FPS. Drops occur in dense areas such as foliage, lava and water.
- **Image quality**: aliasing is visible because anti-aliasing is off.
- **Stability**: no disconnection or crash over the 140-second recording.
- **Noise**: acceptable.
- **Heat**: the headset gets warm during play.

## Reference images

- `images/frame-00s.jpg`, `images/frame-70s.jpg`, `images/frame-105s.jpg`: sample frames
- `images/contact-sheet-gameplay.jpg`: 16 gameplay frames, one every 5 seconds
- `images/contact-sheet-settings.jpg`: 12 settings-menu frames

## Video

[`video/benchmark-minecraft-quest2.mp4`](video/benchmark-minecraft-quest2.mp4), 140 seconds, 1920 × 1080.

## Recommendations

1. Lower render distance to 8 chunks.
2. Turn off heavy effects such as shadows, particles and reflective water.
3. Keep 72 Hz to limit heat.
4. Take regular breaks during long sessions.

## Sources

- [Horizon VR](https://github.com/Boboetto/Horizon-vr): fork of Rayan-XOO/horizon, MIT licence, targets Meta Quest 3.
- [Horizon](https://github.com/Rayan-XOO/horizon): native Rust client for Minecraft Java Edition 26.3, with an Android port that includes a launcher.
- [Quest 2 120 Hz mode is no longer experimental](https://uploadvr.com/quest-2-120hz-no-longer-experimental/)
- [Meta ends Quest 2 OS updates by March 2027](https://techenclave.com/news/items/meta-to-end-quest-2-and-quest-pro-os-updates-by-march-2027)

---

*Written with the help of Claude Haiku 5.5.*
