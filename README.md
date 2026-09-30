# Orbital Laser — 60s Cooldown & Unlimited Uses

Version 1.0.0

Call in the Orbital Laser with a **60-second base cooldown** and **unlimited uses per mission**.

| Setting | Original | Modded |
| --- | ---: | ---: |
| Base cooldown | 300 seconds | 60 seconds |
| Uses per mission | 3 | Unlimited |

Ship upgrades and mission modifiers may adjust the final cooldown. Laser damage,
duration, targeting, and call-in delay remain unchanged. Other stratagems are unaffected.

## Requirements

- Helldivers 2 on Windows x64.
- Bingus Shared Loader v15 or newer / API 1, compatible with your installed game build.
- Arsenal or HD2MM.

## Installation

1. Close Helldivers 2.
2. Import this ZIP into your mod manager.
3. Enable this mod and Bingus Shared Loader. With default Arsenal priority, keep the
   loader last; if using first-mod priority, place it first instead.
4. Purge / Deploy, then launch the game. Allow the startup scan to finish on your ship.

Upgrading from the v0.1.0 test: replace the previous entry; do not enable two copies.
The manager GUID is retained. This corrected package uses a neutral resource identity; remove the previous copy before deploying.
The separate Stratagem Settings Probe is not required.

## Compatibility and troubleshooting

Avoid combining this with another mod that changes the Orbital Laser's cooldown or
use count. Bingus compatibility does not resolve overlapping gameplay edits.
Game updates may require a revised version of this mod.

Status is written to:
`%LOCALAPPDATA%\CowboyBingus\Helldivers2\OrbitalLaser60\STATUS.txt`

Typical Windows path:
`C:\Users\%username%\AppData\Local\CowboyBingus\Helldivers2\OrbitalLaser60\STATUS.txt`

An `OK` result means a matching record was patched and verified. If the timer or
use limit does not change, check this file and include it in a bug report with your
game version and other active gameplay mods. Test cooldown behaviour and a fourth
call-in to verify both effects. A loader message saying `loaded` alone does not prove
that the values were applied.

The scan runs once at startup. If the game reloads these settings later, the patch
may be lost until the next launch. The scan can briefly add startup work; it stops
when finished. Host/client differences and all multiplayer combinations have not
been independently verified.

## Uninstall

Close the game, disable/remove this mod, Purge / Deploy, and restart. Changes are
in memory only; disabling the mod while the game is running does not undo them.

## Release validation

The v0.1.0 gameplay implementation was reported working in-game by the tester on
September 25, 2026. Version 1.0.0 preserves that implementation; only release metadata, documentation, and neutral internal identifiers have changed. An exact game build
number was not supplied with the test report.

Offline tests against a captured stratagem table covered target identification,
changes limited to the two intended fields, repeat application, rejection of
mismatched records, and rollback after simulated write/readback failures.

## Credits

Release project: Miker, with coding and testing assistance from ChatGPT/Codex.
Requires Bingus Shared Loader by CowboyBingus; the loader is distributed separately.
Memory access helpers were adapted from the supplied M6C SOCOM AP4 Durable 60 v2.0.0
addon. Source attribution is retained; this package does not assert ownership of
that upstream work or grant additional rights to it.

Editable source and the offline test script are included as reference files.
They are not deployed by the mod manager. See DEVELOPMENT.md for rebuilding.

If you enjoy my mods and would like to support my work, consider buying me a coffee on Ko-fi! Any support is greatly appreciated. https://ko-fi.com/mikerbiker
