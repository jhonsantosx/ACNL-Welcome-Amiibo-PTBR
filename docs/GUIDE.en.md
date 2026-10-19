# Installation and updates

[Português: instalação](INSTALACAO.md) · [Português: atualização](ATUALIZACAO.md)

## Nintendo 3DS with Luma3DS

1. Start with a working installation of **Welcome amiibo USA**, Title ID `0004000000198E00`.
2. Download the attached translation ZIP from [Releases](https://github.com/jhonsantosx/ACNL-Welcome-Amiibo-PTBR/releases), not the automatic Source code archive.
3. Save and close the game. Power off before removing the SD card.
4. Extract the ZIP and copy **luma** to the SD card root. Merge folders; do not delete the entire existing luma folder.
5. Eject the card, put it back and hold **SELECT** while powering on.
6. Enable **Enable game patching** with **A**, then press **START** to save and boot.
7. Launch the game normally.

The final paths must be:

```text
SD:/luma/titles/0004000000198E00/romfs/Script/...
SD:/luma/titles/0004000000198E00/locale.txt
```

Keep `locale.txt` set to **USA EN**. Portuguese replaces the English language layer. The patch uses [Luma's LayeredFS](https://github.com/LumaTeam/Luma3DS/wiki/Optional-features); it is not installed through FBI.

## Citra

1. Make sure the game already runs.
2. Right-click Welcome amiibo and open its **Mods Location**.
3. From `luma/titles/0004000000198E00/` inside the ZIP, copy **romfs** into that mods folder.
4. Set the emulated system language to **English**. Luma's locale.txt does not configure Citra.
5. Restart the game.

The path should end in `load/mods/0004000000198E00/romfs/Script/…`. Do not copy the entire luma hierarchy into the mods folder.

## Updating

No need to reinstall the game, delete your town or start a new save. Close the game and power off the console, then copy the new patch and overwrite matching files.

If release notes announce removed or reorganized files, back up **only** this game's patch `romfs` folder to your computer, remove it from the SD and replace it with the new one. This avoids stale patch files. Do not delete Nintendo 3DS, the entire luma directory or save folders. Other mods using the same patch directory may conflict.

In Citra, replace the patch romfs while the game is closed. Official game updates are separate from translation updates.

## Troubleshooting and reverting

Check Title ID, folder nesting, English language and Enable game patching. Find your patch version in `VERSAO.txt`. An isolated English sentence may still be a preview limitation.

To revert, restore the previous patch folder. To disable, move the patch out of the loading path. Keep your save.

[Report persistent issues](https://github.com/jhonsantosx/ACNL-Welcome-Amiibo-PTBR/issues/new/choose) with platform, patch version, official game update if any, and screenshots. Full console visual testing remains pending.
