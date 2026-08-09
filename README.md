## Overview

This is a small test PCB to experiment with wide color gamut LEDs. The initial plan is to use the following LEDs, driven by the TI TLC5971 (high-quality 16-bit PWM).

1. Violet 410 (XE-G)
2. Blue PC 460 (OSLON)
3. Cyan 500 (XE-G)
4. Green 525 (OSLON)
5. Yellow PC 590 (OSLON)
6. Red 620 (OSLON)
7. Photo Red 660 (XE-G)
8. Far Red 735 (Luxeon)
9. White (OSLON)

This should allow tests to compare more traditional RGB and RGBW color gamuts to wider gamuts. In particular, deeper reds, violet, and cyan. 

### Cyan
Initial testing shows that the cyan LED makes a color that is perceptually different from just mixing various amounts of green and blue. Green+blue results in the traditional computer monitor "cyan", which is really more turquoise. The pure cyan LED results in a more saturated (computer monitor cyan is a bit pastel by comparison) strong green-blue color.

### Violet

By itself, the violet LED is not what I expected: it seems almost like a purple/blue/white mixture. I need to do more research to make sure it is not exciting the phosphors in the white LED (perhaps build a board without the white). My plans are to compare purples (red+blue and red+violet) to see if violet generates noticeably different (i.e. more intense) purpl

### Photo Red and Far Red

This is an interesting example of how our eyes acclimate, color balance, and otherwise shift our perceptions. When I look at the normal red LED, it looks strongly red. But when I look at normal red next to photo red, the photo red looks more intensely red and the normal red starts to look like an orange-red. I want to try a larger experiment to determine how this effect scales.

The far red appears to be useless for LED sculptures, animations, or lighting. The perceived brightness is MUCH (like 10-20X) lower, so it can only produce very dim illumination. And as seen on the chromaticity diagrams, the perceived color is very close to photo red, so it does not meaningfully increase the gamut.