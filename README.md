# DrawDoodle Bundle Instructions

This project contains an HTML game, **Doodle Draw.html**, along with audio and image assets used by the page. To play the game offline or host it yourself, bundle the HTML file together with the required assets in a single archive.

## Required files

Include `Doodle Draw.html` and the following audio and image files:

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

### Images (`assets/images/*.png`)
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

## Creating the zip archive
1. Place `Doodle Draw.html` in a folder along with all the files listed above.
2. From that folder, run a command like:
   ```bash
   zip -r doodle-draw.zip "Doodle Draw.html" *.mp3 assets/images/*.png
   ```
   This command adds the HTML file, every `.mp3`, and every `.png` inside `assets/images/` into `doodle-draw.zip`.

The HTML references these assets with relative paths, so when you upload or distribute the game, ensure the `.mp3` and `assets/images` files remain in the same directory structure next to `Doodle Draw.html`.
