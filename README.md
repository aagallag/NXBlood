# NXBlood
Switch Blood port based on EDuke32


## Installing
1. put the NRO into the switch directory
2. make a folder called nblood in the root of the SD card
3. Copy the following files from Blood 1.21 to nblood folder:

   BLOOD.INI  
   BLOOD.RFF  
   BLOOD000.DEM-BLOOD003.DEM  
   GUI.RFF  
   SOUNDS.RFF  
   SURFACE.DAT  
   TILES000.ART-TILES017.ART  
   VOXEL.DAT  

4. Copy nblood.pk3 from this repo into the nblood folder
5. Optionally if you want to use CD audio tracks instead of MIDI, provide FLAC/OGG recordings in following format: bloodXX.flac/ogg, where XX is track number. Make sure to enable Redbook audio option in sound menu.
6. Launch NXBlood

## Building NXBlood
# Requirements
Make sure to have setup the devkitarm toolchain with devkita64
install `switch-sdl2 switch-sdl2_mixer switch-libogg switch-libvorbis switch-flac` over pacman
currently the required libFLAC packaged from pacman has undefined references, compile it yourself from https://github.com/devkitPro/pacman-packages

# Building
run `make PLATFORM=SWITCH`

for various compilation options check the the [EDuke32 Wiki]


## Acknowledgments:
### EDuke32 engine & game programming:
  * TerminX
  * Hendricks266
  * pogokeen
  * Plagman
  * Helixhorned
  
### JFDuke3D by:
  * JonoF
  
### Uses BUILD Engine technology by:
  * Ken Silverman
  
### NBlood programming:
  * Nuke.YKT

### Switch port
  * Jan200101

### Additional programming:
  * sirlemonhead
  
### Widescreen tiles & NBlood logo:
  * Maxi Clouds
  
### Special thanks:
  * NY00123, MetHy, Striker, oasiz, Mblackwell, Zombie, Marphy Black, SAmik37, meleemario
