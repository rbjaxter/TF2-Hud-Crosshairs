# Notes on Crosshair Experimentation
Any misc information and anything learned while trying to improve crosshairs will be dumped here.

rough video explaining steps: https://youtu.be/m1UsOo6VKWI

### Exporting Original SVGs
* Open original font in FontForge
* Go to File > Execute Script
* Enter: `SelectWorthOutputting(); foreach Export("svg"); endloop;`
* Select `FF`
* SVGs will be exported to the same place original font is located

Note that this only extracts the lowercase glyphs (the uppercase glyphs have the same file name and get overwritten), so you'll need to come up with some foolery to get the uppercase glyphs as well (I just copied the font, cleared all of the lowercase glyphs, saved it, and then ran the script again).

### Illustrator Setup
* 512px x 512px
* Add guides for absolute center
* This file serves as the template for the next step

### Centering SVGs
* Open original, exported glyph SVG
* Copy original glyph into new template Illustrator file
* With original glyph selected, adjust x/y position (at the top) to 256px x 256px
* This generally does the trick, but manually center the crosshair as necessary
* File > Save As > SVG
* The only value I changed was "Decimal Places" from 1 to 3
* Repeat 50000 times for each glyph