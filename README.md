# DisableUnitChecks

A configuration mod for [Phantom Brigade (Alpha)](https://braceyourselfgames.com/phantom-brigade/) that disables all unit checks in the mobile base unit screen as well as the briefing screen and the squad view right before combat.

It is compatible with RELEASE patch **0.22.2-b4942** and EXPERIMENTAL patch **0.23.1-b5426**.

This should be used only for diagnostics. It will let your units go into combat without parts like legs, arms and even the core.

## Instructions for Use (RELEASE patch only)

0. Make sure the game is not running.
1. Make a `Mods` folder in `C:\Users\<username>\Documents\My Games\Phantom Brigade` if you do not already have one.
2. Download the [mod bundle zip file](https://github.com/echkode/PhantomBrigadeMod_DisableUnitChecks/releases/download/r1/DisableUnitChecksMod.zip) and extract the contents to the `Mods` folder.
3. Download the [mods.yaml file](https://github.com/echkode/PhantomBrigadeMod_DisableUnitChecks/releases/download/r1/mods.yaml) and copy it to `C:\Users\<username>\Documents\My Games\Phantom Brigade\Settings` if you don't already have `mods.yaml` file. If you do, copy the last two lines of the downloaded file into the existing one. Ask on the phantom-modding forum if you have `mods.yaml` and are unsure what to do.
4. Start the game and check the Mods menu to make sure the mod is loaded.
5. Load a saved game and go to the Units screen on the mobile base.
6. Take a good look at your unit to make sure you're not missing something obvious like a small amount of damage or a missing part.
7. Quit the game and go to the `C:\Users\<username>\Documents\My Games\Phantom Brigade\Mods\DisableUnitChecks\ConfigEdits\DataDecomposed\UnitChecks` folder.
8. There will be a set of files with names that should make them pretty obvious what they're for.
9. Delete one of the files with a name that starts with `error_` and then start the game and load your save. Remember the name of the file you deleted.
10. Check the Units screen in the mobile base to see if the error flag has come back.
11. If the error flag reappears, then you know at least one check that is failing. You can stop this troubleshooting process. Quit the game, remove the mod by deleting the `mods.yaml` file and report the failing check through the in-game bug reporter. Don't use the in-game bug reporter if you have any loaded mods.
12. If not, quit the game and go back to step 9. When you run out of `error_` files, pick a file with a name that starts with `warning_` and continue on.

Make sure you remove the mod when you're done troubleshooting. Best to delete the `mods.yaml` and the DisableUnitChecks folder.

## Instructions for Use (EXPERIMENTAL patch)

BYG changed where the user data for the game is stored. Replace all the references to `C:\Users\<username>\Documents\My Games\Phantom Brigade` with `C:\Users\<username>\AppData\Local\PhantomBrigade` and follow the steps for the RELEASE patch.
