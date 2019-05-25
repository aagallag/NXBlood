# NXBlood
a homebrew port of NBLood for the Nintendo Switch

## NBlood

### Installing
1. put the NRO into the switch directory
2. make a folder called nblood in the root of the SD card
3. Copy the following files from Blood 1.21 to nblood folder:

   BLOOD.INI  
   BLOOD.RFF  
   BLOOD000.DEM-BLOOD003.DEM (optional)  
   CP01.MAP-CP09.MAP (optional, Cryptic Passage)  
   CPART07.AR_ (optional, Cryptic Passage)  
   CPART15.AR_ (optional, Cryptic Passage)  
   CPBB01.MAP-CPBB04.MAP (optional, Cryptic Passage)  
   CPSL.MAP (optional, Cryptic Passage)  
   CRYPTIC.INI (optional, Cryptic Passage)  
   CRYPTIC.SMK (optional, Cryptic Passage)  
   CRYPTIC.WAV (optional, Cryptic Passage)  
   GUI.RFF  
   SOUNDS.RFF  
   SURFACE.DAT  
   TILES000.ART-TILES017.ART  
   VOXEL.DAT  

4. Copy nblood.pk3 from this repo into the nblood folder
5. Optionally if you want to use CD audio tracks instead of MIDI, provide FLAC/OGG recordings in following format: bloodXX.flac/ogg, where XX is track number. Make sure to enable Redbook audio option in sound menu.
6. Launch NXBlood

## Building NXBlood
### Requirements
Make sure to have setup the devkitarm toolchain with devkita64
install `switch-sdl2 switch-sdl2_mixer switch-libogg switch-libvorbis switch-flac` over pacman
currently the required libFLAC packaged from pacman has undefined references, compile it yourself from https://github.com/devkitPro/pacman-packages

### Building
run `PATH=$DEVKITPRO/portlibs/switch/bin:$PATH make PLATFORM=SWITCH`

for various compilation options check the the [EDuke32 Wiki]

## PCExhumed
A port of the PC version of Exhumed based on EDuke32

### Installing
1. Extract PCExhumed to a new directory.
2. Copy the following files from the PC retail version of Exhumed or Powerslave (Exhumed preferred), or the Powerslave demo available at http://www.jonof.id.au/build.games/ps. Beta, pre-release or other demo versions not supported.

   STUFF.DAT  
   DEMO.VCR  
   BOOK.MOV  

   The game is unfortunately not currently available for sale. Please provide files from an original release of the game.

3. Recommended (but optional) - Add the games CD audio tracks as OGG files in the format exhumedXX.ogg (where XX is the track number) to the same folder as
   pcexhumed.exe. The game includes tracks 02 to 19.
   These will provide the game with it's awesome music soundtrack and add storyline narration by the King Ramses NPC.

4. Launch PCExhumed.
### Switch port
  * Jan200101


### Notes
Demo playback is not yet working.

### Adjusting settings
We are currently working on fancy new menus for the game. In the meantime, you can edit the settings.cfg file in the game directory that's created on first run.

To invert the mouse, add the line 'in_mouseflip 0' to settings.cfg.
To change the FOV, add a new line to settings.cfg, e.g. 'fov "120"' where 120 is the desired FOV value between 60 and 140.

## Building from source
See: https://wiki.eduke32.com/wiki/Main_Page

## Acknowledgments
  See AUTHORS.md
