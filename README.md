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
1. Download the zip folder and unzip it
2. Locate your starfall directory
   (e.x. `C:\Program Files (x86)\Steam\steamapps\common\GarrysMod\garrysmod\data\starfall`)
3. Copy and paste the files, maintaining the same file hierarchy, into your starfall folder.
    - As a result, your files should look like this:
        - `starfall\lib\modular_hud_base.txt`
        - `starfall\lib\modular_hud_elements_base.txt`
        - `starfall\lib\modular_hud_elements_daktank.txt`
        - `starfall\lib\modular_shared_memory_3.txt`
        - `starfall\lib\modular_wire_helper.txt`
        - `starfall\modular_hud_v1_(public_release)_(daktank).txt`

# Notes:
- The HUD elements aren't completely modular, and could be improved (e.x. autocalculating alignments for text in boxes). At the end of the day, the level of abstraction is up to the user to decide. The HUD elements are just there to provide basic functionality, and to demonstrate what is possible.
- At the time of writing, I have tried my best to optimize the libraries, (and the client/server usages do seem to reflect it), but I won't act like I know everything about optimization. There is always room for improvement.
- Some libraries like the wire helpers offer functionality which could be considered redundant or excessive. If this is the case, feel free to modify what is necessary (e.x. remove the entity valid checks from hud base and you no longer depend on the wire helper library).
