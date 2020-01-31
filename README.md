
![PrusaSlicer logo](/resources/icons/PrusaSlicer.png?raw=true)

# PrusaSlicer 2.1.1 DRIBBLING V.B01

This is a Fork of the PrusaSlicer 2.1.1
You may want to check the [PrusaSlicer project page](https://www.prusa3d.com/prusaslicer/).
For information on PrusaSlicer check the [PrusaSlicer project page](https://www.prusa3d.com/prusaslicer/).
Prebuilt Windows, OSX and Linux binaries are available through the [git releases page](https://github.com/prusa3d/PrusaSlicer/releases) or from the [Prusa3D downloads page](https://www.prusa3d.com/drivers/).

### What are the PrusaSlicer's DRIBBLING features compared to the original PrusaSlicer?

On the Filament tab in Advanced group, in the Toolchange  parameters with single extruder MM printers, there are some additional parameters:

- DRIBBLING MODE (on/off) -> if you do not enable dribbling mode, it works exactly as the standard PrusaSlicer.
- Melting distance (do not change, probably will be hard coded for Prusa printers)
- Number of Dribbling moves

If Dribbling mode is enabled, during the MMU2S filament change, just before extracting the filament, it starts to play with the filament doing a sort of dribbling and each hit of the filament in the melting area shapes the head almost squared, limiting the strings and strange big balls shapes to the minimum. It is possible to vary the effect to tune it with the owned specific filament by changing the parameter 'Number of Dribbling moves'.
I had developed it especially for PLA filaments, in order to use bad quality / low cost filaments spools.
For the moment I decided to do not change the temperature, in order to keep print time short.

See a close-up picture of some filament heads  I got during a MMU2 multicolour print.
![heads](/heads.jpg?raw=true)

### Development

If you want to compile the source yourself, follow the instructions on one of
these documentation pages:
* [Linux](doc/How%20to%20build%20-%20Linux%20et%20al.md)
* [macOS](doc/How%20to%20build%20-%20Mac%20OS.md)
* [Windows](doc/How%20to%20build%20-%20Windows.md)

### What's PrusaSlicer license?

PrusaSlicer is licensed under the _GNU Affero General Public License, version 3_.
The PrusaSlicer is originally based on Slic3r by Alessandro Ranellucci.

### How can I use PrusaSlicer from the command line?

Please refer to the [Command Line Interface](https://github.com/prusa3d/PrusaSlicer/wiki/Command-Line-Interface) wiki page.
