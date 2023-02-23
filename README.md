# ModularHud
An implementation of a modular HUD in SF for Garry's Mod

# Motivation
- Public SF HUDs for ACF/Daktank have not proliferated nearly as much as I thought they would
- Taking advantage of SF's distinction between client and server to achieve better optimization than E2 can offer for the same capabiliities

# Demo
![image](https://user-images.githubusercontent.com/109800352/210301162-1db72574-db24-42d1-9156-e32a79638dbd.png)

# Status
- Currently only a daktank example hud has been created. If the time presents itself, an ACF example may be made.

# Installation Instructions:
- [ACF](https://github.com/LengthenedGradient/ModularHud/wiki/ACF-HUD-Setup-Guide)
- [Daktank](https://github.com/LengthenedGradient/ModularHud/wiki/Daktank-HUD-Setup-Guide)

# Notes:
- The HUD elements aren't completely modular, and could be improved (e.x. autocalculating alignments for text in boxes). At the end of the day, the level of abstraction is up to the user to decide. The HUD elements are just there to provide basic functionality, and to demonstrate what is possible.
- At the time of writing, I have tried my best to optimize the libraries, (and the client/server usages do seem to reflect it), but I won't act like I know everything about optimization. There is always room for improvement.
    - I can guarantee the optimizations of the example HUDs; not so much any modifications made after. I have included tips for optimization in the FAQ of the wiki.
- Some libraries like the wire helpers offer functionality which could be considered redundant or excessive. If this is the case, feel free to modify what is necessary (e.x. remove the entity valid checks from hud base and you no longer depend on the wire helper library).
