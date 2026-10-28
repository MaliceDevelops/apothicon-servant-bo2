# Changelog

## 4.2

Sounds remixed to match Black Ops 3, BO3's crosshair, and a quieter creature.

- **Sounds match BO3.** Every sound's volume and range now come from BO3's own sound data. Before, the black hole could barely be heard more than a few steps away. Now you hear it open, hum and collapse from across the room, and it gets louder as you get closer.
- **BO3's extra sound layers:** the bass hit under the black hole opening and under its explosion, and the explosion's extra crack.
- **Louder:** the creature's greeting, its reload, and zombies being pulled in and crushed.
- **Quieter:** the creature's wet idle noise while you hold the gun.
- **Crosshair:** BO3's own Apothicon Servant crosshair, with the square in the middle.
- **The creature talks like in BO3:** it greets you when you get the gun, and that's all. Its combat and idle lines are in BO3's files, but BO3 never plays them. To hear them anyway, turn on the new `creature_chatter` setting (see the README's Settings).
- **New installer:** Install.bat opens a window with a tick box for each of my mods (the Apothicon Servant and the [Upgraded Cymbal Monkey](https://github.com/MaliceDevelops/upgraded-cymbal-monkey-bo2) so far). Only the ticked ones are downloaded, each from its own GitHub page, and they all work together in the same game, with or without Zombies Declassified. With Zombies Declassified they leave its second fastfile slot free for someone else's mod. It stays on your PC with a "MaliceDevelops BO2 Mods" shortcut (desktop and Start menu) to add, remove or update mods, change their settings (with Reset to defaults), repair a broken install, or turn the mods off so Zombies Declassified plays as it came. It updates itself when a newer installer is out. It takes over an install from an earlier version (by Install.bat or by hand) and keeps your settings. It needs an internet connection.
- The download now unzips correctly on Linux and Steam Deck (folders used to show up as long file names).

Updating keeps your settings file as it was, so it has no `creature_chatter` line. The README's Settings section shows the line to add.

## 4.1.1

Installer fixes. The gun itself is unchanged.

- Install.bat now recognises a copy you installed by hand (following the README's "install by hand" steps). It updates that copy and keeps your settings, instead of setting its file aside as another mod's. If you have Zombies Declassified, it also removes a hand-made separate "Apothicon Servant" mod, so the Mods menu has no second entry.
- Uninstall.bat also removes a copy installed by hand.

## 4.1

The black hole now catches zombies the way Black Ops 3's does:

- It pulls in every zombie in range, including ones behind walls, ones outside the map walking up to a window, and ones tearing at its boards. A zombie at a window lets go, and the board it was pulling goes back.
- A zombie that's rising out of the ground, climbing through a window or jumping down finishes that first, then gets pulled in.
- Zombies the game is still spawning are left alone until they're in place, so none pop up out of nowhere.
- The explosion kills every zombie in range, including ones still rising out of the ground.
- The download now links to this page for updates.

## 4.0

First public release.
