# gbafreedoom
AI辅助移植版
GBAfreeDoom

A port of prBoom to the GBA.

What's hot?

Supports Doom Shareware, Retail, Ultimate and Doom2 IWADS. Plutonia and TNT should mostly work.

No WAD is built into the ROM. GbaWadUtil patches a WAD into the prebuilt engine ROM, with no compiler needed. PWADs (Eg: Sigil) go on top of their IWAD.

Renderer is intact, including Doom's distance lighting and full resolution floors and ceilings.

Monster behaviour is all intact. (I.e sound propagation etc.)

Framerate is pretty variable. Simple areas run at ~35fps and complex areas slow down, but V3's renderer is much faster than earlier versions. Doom1 Episodes 1-3 are all completely playable.

Music and sound effects come from the WAD: the game's own music, played with GUS instrument patches, and its own sound effects. PWADs with custom music and sounds work.

Vanilla DeHackEd patches. GbaWadUtil applies a WAD's DEHACKED lump, or a .deh file with -deh, when it builds the ROM.

What's not?

My Markdown skills.

Demo compatibility is broken.

General optimisation. We're never going to get a perfect 35FPS but I think there is still another 25% left without changing the visual quality/correctness/game behaviour. For reference, the first time I ran a build under the emulator it ran at about 3FPS.

Although it is based on prBoom, most of the engine enhancements (BEX, limit removing etc) have been reverted back to Vanilla. This is either for memory or performance reasons. Sadly, NUTS.wad and Okuplok are right out! Binary DeHackEd patches aren't supported either.

No multiplayer.

KippyKip is maintaining an upstream fork with new features and fixes. KippyKip GBA fork

Cheats:

Chainsaw: L, UP, UP, LEFT, L, SELECT, SELECT, UP
God mode: UP, UP, DOWN, DOWN, LEFT, LEFT, RIGHT, RIGHT
Ammo & Keys: L, LEFT, R, RIGHT, SELECT,UP, SELECT, UP
Ammo: R, R, SELECT,R, SELECT,UP, UP, LEFT
No Clipping: UP, DOWN, LEFT, RIGHT, UP, DOWN, LEFT, RIGHT
Invincibility: A, B, L, R, L, R, SELECT, SELECT
Berserk: B, B, R, UP, A, A, R, B
Invisibility: A, A, SELECT,B, A, SELECT, L, B
Auto-map: L, SELECT,R, B, A, R, L, UP
Lite-Amp Goggles: DOWN,LEFT, R, LEFT, R, L, L, SELECT
Exit Level: LEFT,R, LEFT, L, B, LEFT, RIGHT, A
Toggle FPS counter: A, B, L, UP, DOWN, B, LEFT, LEFT

Controls:

Fire: B
Use / Sprint: A
Walk: D-Pad
Strafe: L & R
Automap: SELECT
Weapon up: A + R
Weapon down: A + L
Menu: Start

