# Meta Quest 2 Benchmark: Minecraft Java via Horizon VR

Performance test of Minecraft Java Edition running through Horizon VR on a Meta Quest 2 in standalone mode.

## Setup

| Item | Value |
|---|---|
| Headset | Meta Quest 2 (standalone) |
| OS | Latest version |
| VR app | Horizon VR (unofficial VR port of the Horizon client) |
| Game | Minecraft Java Edition 26.3 |
| Graphics API | Vulkan |
| Refresh rate | 72 Hz |
| Max framerate | 120 FPS |
| VSync | On |
| Anti-aliasing | Off |
| Resolution scale | 85% |

## Settings used (from the in-game menus)

Values read from the settings screens recorded in the video (see the reference images below).

### General

| Setting | Value |
|---|---|
| Preset | Custom |
| Render distance | 16 chunks |
| LOD distance | Off |
| Far detail | Reduced |
| Simulation distance | 6 chunks |
| Brightness | Auto |
| GUI scale | Auto |
| Fullscreen mode | Exclusive fullscreen (current) |
| VSync | On |
| Max framerate | 120 FPS |
| Reduce FPS when | AFK |

### Quality

| Setting | Value |
|---|---|
| Sky | On |
| Fog | On |
| Weather | On |
| Weather effect radius | 10 blocks (Decreased) |
| Particles | Decreased |
| Hide block-break particles | On |
| Smooth lighting | On |
| Biome blend | 3×3 (Fast) |
| Entity distance | 75% |
| Entity shadows | On |
| Show vignette | On |
| Chunk fade | 0.75 s |
| Mipmap levels | 1 |
| Texture filtering | Anisotropic 8× |
| See-through leaves | On |
| Improved transparency | On |
| Animated textures | On |
| Resolution scale | 85% |
| Anti-aliasing | Off |

### Performance

| Setting | Value |
|---|---|
| Chunk updates | Unlimited |
| Upload budget | Unlimited |
| Worker threads | Auto (3) |
| Cave culling | On |
| GPU culling | Off |
| Entity culling | Off |
| Particle culling | Off |
| Entity culling precheck | 64 mobs |
| Leaf culling | Off |
| Block entities: shulker boxes, signs, decorated pots, bells, chests, banners | On |

### Interface

| Setting | Value |
|---|---|
| Attack indicator | Crosshair |
| Autosave indicator | On |

### Advanced

| Setting | Value |
|---|---|
| Present mode | Efficient |
| Frame pacing | Auto (WSync) |
| Graphics API | Vulkan |
| Performance overlay | FPS and graph |

### HDR

| Setting | Value |
|---|---|
| HDR output | On |
| Brightness | Auto (0.00) |
| Peak brightness | Auto (1000) |
| Paper white | Auto (203) |
| UI brightness | 100% |
| HDR lighting | On |

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

Settings screens (read from the video):

- `images/settings/settings-sheet-1-general-distance.jpg`: General and distance settings
- `images/settings/settings-sheet-2-display-quality.jpg`: Display and quality settings
- `images/settings/settings-sheet-3-quality-performance.jpg`: Quality and performance settings
- `images/settings/settings-sheet-4-advanced-hdr.jpg`: Advanced and HDR settings

Gameplay:

- `images/frame-00s.jpg`, `images/frame-70s.jpg`, `images/frame-105s.jpg`: sample frames
- `images/contact-sheet-gameplay.jpg`: 16 gameplay frames, one every 5 seconds

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
