# Benchmark Meta Quest 2 : Minecraft (Horizon VR) — FR / EN

Ce dépôt documente un test de performance d'un Meta Quest 2 avec Minecraft, avec les paramètres utilisés, des images de référence et la vidéo d'origine.

This repository documents a performance test of a Meta Quest 2 running Minecraft, with the settings used, reference images and the original video.

> ⚠️ **Incohérence à lire en premier / Important discrepancy:** la vidéo ne montre pas une session Horizon Client streamée depuis un PC. Elle montre un monde de type Minecraft, filmé sur écran plat, avec un overlay de performances affichant des FPS supérieurs à 90, ce qui est impossible sur un Quest 2 (limité à 90 Hz, 120 Hz en mode expérimental). Les chiffres ci-dessous sont donc **indicatifs**.
>
> The video does not show a Horizon Client session streamed from a PC. It shows a Minecraft-style world captured from a flat screen, with a performance overlay reporting FPS above 90, which a Quest 2 cannot display (90 Hz maximum, 120 Hz experimental). The figures below are therefore **indicative only**.

---

## Sommaire / Contents

1. [Fiche de test / Test setup](#1-fiche-de-test--test-setup)
2. [Paramètres utilisés / Settings used](#2-paramètres-utilisés--settings-used)
3. [Résultats / Results](#3-résultats--results)
4. [Images de référence / Reference images](#4-images-de-référence--reference-images)
5. [Vidéo / Video](#5-vidéo--video)
6. [Chaleur et bruit / Heat and fan noise](#6-chaleur-et-bruit--heat-and-fan-noise)
7. [Recommandations / Recommendations](#7-recommandations--recommendations)
8. [Sources et références / Sources](#8-sources-et-références--sources)

---

## 1. Fiche de test / Test setup

| Élément / Item | Valeur / Value |
|---|---|
| Casque / Headset | Meta Quest 2 |
| Mode / Mode | Standalone (déclaré par l'auteur / reported by the author) |
| OS | Dernière version / latest version (numéro exact à compléter / exact build to fill in) |
| Fréquence d'affichage / Refresh rate | 72 Hz |
| Anticrénelage / Anti-aliasing | Désactivé / Off |
| Jeu / Game | Minecraft (Java Edition, version à compléter / version to fill in) |
| Application VR / VR app | Horizon VR, non officielle, conçue pour le Quest 3 / unofficial, built for the Quest 3 |
| Durée de l'enregistrement / Recording length | 140 s |
| Résolution vidéo / Video resolution | 1920 × 1080, HEVC, environ 30 i/s / fps |

**Note** : le projet Horizon VR cible le Quest 3. Son utilisation sur Quest 2 n'est pas garantie. / The Horizon VR project targets the Quest 3. Its use on a Quest 2 is not guaranteed.

---

## 2. Paramètres utilisés / Settings used

Paramètres lisibles à l'écran sur les captures de la vidéo, à confirmer / Settings readable on the video captures, to be confirmed:

| Catégorie / Category | Réglage / Setting | Valeur observée / Observed value |
|---|---|---|
| Graphismes / Graphics | Distance de rendu / Render distance | 16 chunks |
| Graphismes / Graphics | Distance de simulation / Simulation distance | 6 chunks |
| Graphismes / Graphics | Luminosité / Brightness | Auto |
| Graphismes / Graphics | Distance LOD / LOD distance | À confirmer / to confirm |
| Qualité / Quality | Fondu des chunks / Chunk fade | 0,75 s |
| Performance / Performance | Limite de FPS / Max framerate | À confirmer / to confirm |
| Performance / Performance | VSync | Activé / On |
| Performance / Performance | Culling des entités, grottes, particules / Entity, cave and particle culling | Activé / On |
| Avancé / Advanced | Mode de rendu / Render mode | À confirmer / to confirm |

Les options de mod (LOD, Far Detail, Bluestar Radius) ressemblent à celles du mod **Distant Horizons**. / The mod options (LOD, Far Detail, Bluestar Radius) resemble those of the **Distant Horizons** mod.

---

## 3. Résultats / Results

Valeurs lues sur l'overlay de la vidéo, approximatives / Values read from the video overlay, approximate:

| Mesure / Metric | Résultat / Result | Lecture à 72 Hz / Reading at 72 Hz |
|---|---|---|
| FPS affichés / Displayed FPS | Environ 35 à 170 i/s / about 35 to 170 fps | Au-dessus de 72 : surplus inutile sur le casque / above 72: wasted on the headset |
| Temps de frame / Frame time | Environ 6 à 28 ms / about 6 to 28 ms | Budget à 72 Hz : 13,9 ms / budget at 72 Hz: 13.9 ms |
| Chutes / Drops | Zones denses (végétation, lave, eau) / dense areas (foliage, lava, water) | Sous 72 i/s : saccades / below 72 fps: stutter |
| Stabilité / Stability | Aucune déconnexion sur 140 s / no disconnection in 140 s | Constatée / observed |
| Qualité d'image / Image quality | Crénelage visible (AA désactivé) / aliasing visible (AA off) | Faible à modérée / low to moderate |

### Notes indicatives / Indicative scores

| Critère / Criterion | Note / Score |
|---|---|
| Performance | 6/10 |
| Qualité d'image / Image quality | 5/10 |
| Stabilité / Stability | 7/10 |
| Chaleur et bruit / Heat and noise | 4/10 (ressenti / reported) |
| **Global** | **5,5/10** |

Ces notes sont indicatives et ne remplacent pas une mesure dans le casque. / These scores are indicative and do not replace a measurement inside the headset.

---

## 4. Images de référence / Reference images

| Fichier / File | Contenu / Content |
|---|---|
| `images/frame-00s.jpg` | Image à 0 s / frame at 0 s |
| `images/frame-70s.jpg` | Image à 70 s / frame at 70 s |
| `images/frame-105s.jpg` | Image à 105 s / frame at 105 s |
| `images/contact-sheet-gameplay.jpg` | Planche de 16 images de jeu (une toutes les 5 s) / contact sheet of 16 gameplay frames (one every 5 s) |
| `images/contact-sheet-settings.jpg` | Planche de 12 images des menus de réglages / contact sheet of 12 settings-menu frames |

---

## 5. Vidéo / Video

Fichier / File : [`video/benchmark-minecraft-quest2.mp4`](video/benchmark-minecraft-quest2.mp4) (53 Mo / 53 MB, 140 s).

---

## 6. Chaleur et bruit / Heat and fan noise

Ces points ne sont pas mesurables sur la vidéo. Le ressenti de l'auteur : casque chaud, ventilateur trop bruyant. / These points cannot be measured from the video. The author reports: headset gets hot, fan too loud.

**Protocole recommandé / Recommended protocol :**
1. Session de 20 min, puis noter la chaleur à la face, à l'arrière et sur le côté. / 20-minute session, then note the heat at the face, back and side.
2. Mesure du bruit au sonomètre à 30 cm, en dB, à froid puis après 20 min. / Noise measured with a sound meter at 30 cm, in dB, cold and after 20 min.
3. Noter si le ventilateur accélère par à-coups. / Note whether the fan speeds up in bursts.

---

## 7. Recommandations / Recommendations

1. Réduire la distance de rendu à 8 chunks. / Lower render distance to 8 chunks.
2. Désactiver les effets lourds (ombres, particules, eau réfléchissante). / Disable heavy effects (shadows, particles, reflective water).
3. Garder 72 Hz pour limiter la chaleur. / Keep 72 Hz to limit heat.
4. Faire des pauses régulières. / Take regular breaks.
5. Vérifier la version de l'OS et de Minecraft. / Check the OS and Minecraft versions.

---

## 8. Sources et références / Sources

- Projet Horizon VR (GitHub) : <https://github.com/Boboetto/Horizon-vr>, fork de Rayan-XOO/horizon, licence MIT, cible le Quest 3. / Horizon VR project: fork of Rayan-XOO/horizon, MIT licence, targets the Quest 3.
- Discussion Reddit r/MetaQuestVR : <https://www.reddit.com/r/MetaQuestVR/comments/1xuuihw/comment/19spq2ratn0ck/> (non lue par l'auteur de ce README / not read by the author of this README).

---

*Benchmark rédigé avec l'aide de Claude Haiku 5.5.*
*Benchmark written with the help of Claude Haiku 5.5.*
