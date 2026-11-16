# Meta Quest 2 Benchmark: Minecraft Java via Horizon VR

This repository documents a performance test of Minecraft Java Edition on a Meta Quest 2, with the settings used, reference images and the original video.

> **Note:** The video shows a Minecraft-style world captured from a flat screen with a performance overlay. The Meta Quest 2 refresh rate is capped at 120 Hz, so readings above 120 FPS are not valid and have been removed from this benchmark. The game is run at 72 Hz.

---

## 1. Test setup

| Item | Value |
|---|---|
| Headset | Meta Quest 2 |
| Mode | Standalone |
| OS | Latest version (exact build to be filled in) |
| Refresh rate | 72 Hz |
| Anti-aliasing | Off |
| Game | Minecraft Java Edition 26.3, through the Horizon client (exact version to be filled in) |
| VR app | Horizon VR (unofficial VR port of the Horizon client, MIT licence) |
| Recording length | 140 s |
| Video | 1920 × 1080, HEVC, about 30 fps |

**Compatibility note:** The Horizon VR project states it targets the Meta Quest 3. Compatibility with the Quest 2 is not guaranteed.

---

## 2. Settings used

Settings readable on the video captures (to be confirmed):

| Category | Setting | Observed value |
|---|---|---|
| Graphics | Render distance | 16 chunks |
| Graphics | Simulation distance | 6 chunks |
| Graphics | Brightness | Auto |
| Graphics | LOD distance | To be confirmed |
| Quality | Chunk fade | 0.75 s |
| Performance | Max framerate | To be confirmed |
| Performance | VSync | On |
| Performance | Entity, cave and particle culling | On |
| Advanced | Render mode | To be confirmed |

The LOD options (LOD distance, Far Detail, Bluestar Radius) resemble those of the Distant Horizons mod.

---

## 3. Results

Values read from the video overlay, limited to the range the Quest 2 can display (up to 120 Hz):

| Metric | Result |
|---|---|
| Displayed FPS | Roughly 35 to 120 fps, with most scenes near or above 72 fps |
| Frame time | About 8 ms to 28 ms in the valid range |
| Drops | Dense areas (foliage, lava, water) fall below 72 fps |
| Stability | No disconnection or crash in 140 s |
| Image quality | Aliasing visible (anti-aliasing off), low to moderate |

### Scores

| Criterion | Score |
|---|---|
| Performance | 8/10 |
| Image quality | 5/10 |
| Stability | 7/10 |

Scores are indicative and do not replace measurements taken inside the headset.

### Heat and noise

- **Noise:** acceptable according to the author's latest feedback.
- **Heat:** the author reports that the headset gets warm. This has not been measured yet.

---

## 4. Reference images

| File | Content |
|---|---|
| `images/frame-00s.jpg` | Frame at 0 s |
| `images/frame-70s.jpg` | Frame at 70 s |
| `images/frame-105s.jpg` | Frame at 105 s |
| `images/contact-sheet-gameplay.jpg` | 16 gameplay frames, one every 5 s |
| `images/contact-sheet-settings.jpg` | 12 settings-menu frames |

---

## 5. Video

File: [`video/benchmark-minecraft-quest2.mp4`](video/benchmark-minecraft-quest2.mp4) (53 MB, 140 s).

---

## 6. Information still missing

- Exact Quest 2 OS build
- Exact Minecraft Java version
- Horizon VR version and Horizon client version
- Max framerate and LOD settings
- Measured headset temperature and noise level (dB at 30 cm)
- Whether the recording was captured on the headset or on a PC

---

## 7. Recommendations

1. Lower render distance to 8 chunks.
2. Disable heavy effects (shadows, particles, reflective water).
3. Keep 72 Hz to limit heat.
4. Take regular breaks during long sessions.
5. Record the exact OS and game versions.

---

## 8. Sources

- Horizon VR project (GitHub): <https://github.com/Boboetto/Horizon-vr>. Fork of Rayan-XOO/horizon, MIT licence, targets the Meta Quest 3.
- Original Horizon project (GitHub): <https://github.com/Rayan-XOO/horizon>. Native Rust client for Minecraft Java Edition 26.3, with an Android port that includes a launcher.
- Quest 2 120 Hz mode is no longer experimental: <https://uploadvr.com/quest-2-120hz-no-longer-experimental/>
- Meta ends Quest 2 OS updates by March 2027: <https://techenclave.com/news/items/meta-to-end-quest-2-and-quest-pro-os-updates-by-march-2027>
- QuestCraft (unofficial Minecraft Java on Quest 2): <https://www.pcgamer.com/uk/questcraft-makes-minecraft-java-edition-playable-on-quest-2/>
- Reddit r/MetaQuestVR discussion: <https://www.reddit.com/r/MetaQuestVR/comments/1xuuihw/comment/19spq2ratn0ck/> (not read by the author of this README)

---

*Benchmark written with the help of Claude Haiku 5.5.*
