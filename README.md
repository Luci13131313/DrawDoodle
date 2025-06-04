# DrawDoodle Bundle Instructions

This repository contains `Doodle Draw.html` along with the audio and image assets it expects. To run the game on [Farcade](https://farcade.com/) or offline, all of these files must live directly in the zip archive with no extra top-level folder.

## Required files

### Audio (`.mp3`)
- Crash.mp3
- Levelup.mp3
- Scarlatti-sonata-no-1.mp3
- baroque-summer.mp3
- burgmuller-friedrich-innocence-op-100-no-5.mp3
- chopin-prelude-no-11-opus-28.mp3
- chopin-prelude-no-7-opus-28-200772.mp3
- gymnopedie-no-1-erik-satie.mp3
- schumann-scenes-from-childhood-09-on-the-rocking-horse-202087.mp3

### Images (`assets/images/`)
- assets/images/Balloon.png
- assets/images/BoomBox.png
- assets/images/Crown.png
- assets/images/Deysi.png
- assets/images/Hap.png
- assets/images/HapMello.png
- assets/images/Hue.png
- assets/images/IceCream.png
- assets/images/Lolly.png
- assets/images/MediHap.png
- assets/images/Pencil.png
- assets/images/Pickle.png
- assets/images/Pigeon.png
- assets/images/Poop.png
- assets/images/Robot.png
- assets/images/RunHap.png
- assets/images/Snail.png
- assets/images/Stoke.png
- assets/images/Verified.png
- assets/images/WizardHat.png
- assets/images/doopie 04.png
- assets/images/doopie01.png
- assets/images/doopie04.png
- assets/images/DoodlesBG.jpg

## Packaging for Farcade
1. Place `Doodle Draw.html` and every file listed above into a single folder.
2. **From inside that folder**, run:
   ```bash
   zip -r doodle-draw.zip "Doodle Draw.html" *.mp3 assets/images/*
   ```
   Running the command from inside ensures the archive does not contain an extra parent directory.

Upload `doodle-draw.zip` to Farcade. Because the archive has no top-level folder, relative paths like `baroque-summer.mp3` and `assets/images/Hap.png` resolve correctly.
