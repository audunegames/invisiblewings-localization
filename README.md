# Localization resources for Invisible Wings: Chapter One

This repository contains the locale files that are used in [Invisible Wings: Chapter One](https://invisiblewingsgame.com/), a visual novel about Dawn, a young woman of faerie descent, and her quest for answers to her own identity and self-acceptance.

## Structure of a locale file

Each locale file is a YAML file that contains two YAML documents: one for the settings and one for the localized values, referred to as the table.

The settings document contains the information about the locale:

Key           | Description
------------- | -----------
`code`        | The  ISO 639-1 code of the language. See [Wikipedia](https://en.wikipedia.org/wiki/List_of_ISO_639-1_codes) for a list of possible codes.
`steamCode`   | The Steam API language code of the locale. See the [SteamWorks documentation](https://partner.steamgames.com/doc/store/localization#supported_languages) for a list of possible codes.
`displayName` | The English name of the locale.
`nativeName`  | The native name of the locale, as displayed in the options menu in the game.


The table document is a big mapping of localization keys to translated values in the corresponding locale. The top level mapping contains several prefix keys, such as `Menu/OptionsMenu` and `Chapter_1/Dialogue`. These keys in turn contain the mapping of the actual keys.

The structure of the locale file is pretty self-explanatory, but should you have trouble with the format, please reach out to Audune Games, so we can help you!

## Creating a new translation

To create a new fan translation of Invisible Wings, do the following:

1. Create a new locale file according to the above defined structure. You can use the already available locales as examples for the structure.
2. Place the locale file in the directory `StreamingAssets\Localization` relative to your Invisible Wings installation folder.
3. If everything is set up correctly in your locale file, the locale should now appear in the options menu of Invisible Wings. If not, you can see any errors in the log file located at `AppData\LocalLow\Audune Games\Invisible Wings\Player.log` relative to your user directory.

To submit a new fan translation to this repository for possible inclusion in the base game, please create a pull request to this repository for each translation you want to add. Audune Games will approve pull requests and including them in the base game on a case-by-case basis.
