# Draw the Doodles

A cozy drawing game built for **[Remix](https://remix.gg)** — sketch alongside a
cast of doodle characters, set to classical piano.

🎮 **[Play it on Remix »](https://remix.gg/g/fc8d3974-d99f-4341-8f12-5d0d91162dca)**

## About
Draw, score and climb the board with a charming crew of doodles (Hap, Deysi, Hue
and friends) and a soundtrack of Chopin, Satie and Schumann. Mobile-first, portrait.

## Stats
_As of June 2026 — pulled with [remix-creator-analytics](https://github.com/Luci13131313/remix-creator-analytics):_
- **75K+** recorded plays
- **14.7K** unique players
- High score: **1,119,006**

## Tech
- Single-file HTML5 game (`Doodle Draw.html`) + image and audio assets
- Integrated with the Remix SDK (leaderboard, game-over, mute)

---
Made by **[Luci](https://github.com/Luci13131313)** · Built with Remix 🐰

---

## Build / packaging (legacy)

> Notes from when assets were bundled and uploaded manually (pre-Remix asset hosting).

This repository contains `Doodle Draw.html` along with the audio and image assets it expects. To run the game offline or as a bundle, all of these files must live directly in the zip archive with no extra top-level folder.

### Required files

**Audio (`.mp3`):** Crash, Levelup, Scarlatti-sonata-no-1, baroque-summer, burgmuller-friedrich-innocence-op-100-no-5, chopin-prelude-no-11-opus-28, chopin-prelude-no-7-opus-28-200772, gymnopedie-no-1-erik-satie, schumann-scenes-from-childhood-09-on-the-rocking-horse-202087

**Images (`assets/images/`):** Balloon, BoomBox, Crown, Deysi, Hap, HapMello, Hue, IceCream, Lolly, MediHap, Pencil, Pickle, Pigeon, Poop, Robot, RunHap, Snail, Stoke, Verified, WizardHat, doopie 04, doopie01, doopie04, DoodlesBG.jpg

### Packaging
1. Place `Doodle Draw.html` and every file above into a single folder.
2. **From inside that folder**, run:
   ```bash
   zip -r doodle-draw.zip "Doodle Draw.html" *.mp3 assets/images/*
   ```
   Running the command from inside ensures the archive does not contain an extra parent directory, so relative paths like `baroque-summer.mp3` and `assets/images/Hap.png` resolve correctly.
