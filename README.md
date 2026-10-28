# Apothicon Servant for BO2 Zombies (Plutonium)

The Apothicon Servant from Black Ops 3's Shadows of Evil, ported to Black Ops 2 Zombies with its original model, animations, sounds and effects.

### [⬇ Download the latest version](https://github.com/MaliceDevelops/apothicon-servant-bo2/releases/latest)

Under **Assets**, download `Apothicon_Servant_v<version>.zip`.

## How it works

- **Mystery Box.** It follows BO2's wonder weapon rules: only one can be in play at a time. Each game the box has one of BO3's four: Kor-Maroth, Mar-Astagua, Nar-Ullaqua or Lor-Zarozzor.
- **Black hole.** Fire it and a black hole opens where the orb lands. Like in BO3, it drags in every zombie in range, including ones behind walls or outside the windows. It crushes them, then collapses in an explosion that kills the zombies around it.
- **Pack-a-Punch** turns it into the red **Arbgwaoth** version: longer black holes, bigger reach, more ammo.
- **Specials.** Hellhounds, Nova crawlers, monkeys, leapers, ghosts and denizens get pulled in too. **Bosses** (Brutus, Panzer Soldat...) aren't: they're held in place while the black hole is open and lose some health. Avogadro gets knocked back.
- **Maps.** It works on every BO2 zombies map, and on every **Zombies Declassified** map if you have it.

## Install

1. Close Black Ops 2.
2. Unzip the download anywhere and double-click **Install.bat**.
3. Play. The installer checks for Zombies Declassified by itself:
   - **With Zombies Declassified:** launch it like always. The gun is in the box on its maps and on the normal BO2 maps.
   - **Without it:** start Zombies, open **Mods**, pick **Apothicon Servant**, then play any map.

Install.bat needs Windows 10 or 11. To install by hand instead, follow `README.txt` in the download.

Windows may warn about running a downloaded `.bat`. Install.bat only copies the mod's files; you can read `installer\install.ps1` to check.

## Update

Download the newest version from the link above, close BO2 and run its **Install.bat**. It replaces the old version and keeps your settings.

## Uninstall

Close BO2 and double-click **Uninstall.bat**. It removes exactly what Install.bat added and puts back anything it set aside.

## Settings

Open `scripts\zm\zzz_aps_config.gsc` with Notepad. Install.bat shows where it is. You can:

- turn the gun off on chosen maps,
- turn Pack-a-Punch off,
- turn off the Pack-a-Punch camo,
- let the creature say its combat and idle lines too (`creature_chatter`). It's off by default: in BO3 the creature only greets you when you get the gun.

Save, then start a new game.

Updating from 4.1.1 or older keeps your old settings file, which has no `creature_chatter` line. To turn it on, add this line under the `pack_a_punch_camo` line:

```
level.aps_config[ "creature_chatter" ] = 1;
```

## Good to know

- **Co-op:** everyone in the game needs the mod installed.
- **Other mods:** script mods like B2OP work fine alongside it.
- **One fastfile mod in ZD:** Zombies Declassified only has room for **one** mod with its own fastfile (`mods\dlc5\mod_patch.ff`). If you already have one, the installer sets it aside, and Uninstall.bat puts it back. Only one of the two works at a time.
- **With the [Upgraded Cymbal Monkey](https://github.com/MaliceDevelops/upgraded-cymbal-monkey-bo2):** it needs that slot too, so the two can't both be in Zombies Declassified. If the monkey mod is already there, Install.bat offers to install the Apothicon Servant as its own mod instead (Mods menu, normal BO2 maps).
- **Installed another fastfile mod later:** maps can fail to load. Run this mod's Uninstall.bat, or its Install.bat to switch back to it.
- **After a Zombies Declassified update or install:** if the gun is missing from the box, run Install.bat again.

## Bugs

Open an [issue](https://github.com/MaliceDevelops/apothicon-servant-bo2/issues). Include:

- the map,
- whether you have Zombies Declassified,
- the line starting with `APS >>` from `%LOCALAPPDATA%\Plutonium\storage\t6\main\console_zm.log`.

## Changes

See [CHANGELOG.md](CHANGELOG.md).

## Credits

Ported by **MaliceKy**. Built with [OpenAssetTools](https://github.com/Laupetin/OpenAssetTools) and [Plutonium](https://plutonium.pw).

The Apothicon Servant's model, animations, sounds and effects are © Activision / Treyarch, from Call of Duty: Black Ops III. This is a free fan mod, not affiliated with or endorsed by Activision. Don't sell it.
