# Introduce Me

![Latest Release Download Count](https://img.shields.io/github/downloads/p4535992/foundryvtt-introduce-me/latest/module.zip?color=2b82fc&label=DOWNLOADS&style=for-the-badge)

[![Forge Installs](https://img.shields.io/badge/dynamic/json?label=Forge%20Installs&query=package.installs&suffix=%25&url=https%3A%2F%2Fforge-vtt.com%2Fapi%2Fbazaar%2Fpackage%2Fintroduce-me&colorB=006400&style=for-the-badge)](https://forge-vtt.com/bazaar#package=introduce-me)

![Foundry Core Compatible Version](https://img.shields.io/badge/dynamic/json.svg?url=https%3A%2F%2Fraw.githubusercontent.com%2Fp4535992%2Ffoundryvtt-introduce-me%2Fmaster%2Fsrc%2Fmodule.json&label=Foundry%20Version&query=$.compatibility.verified&colorB=orange&style=for-the-badge)

![Latest Version](https://img.shields.io/badge/dynamic/json.svg?url=https%3A%2F%2Fraw.githubusercontent.com%2Fp4535992%2Ffoundryvtt-introduce-me%2Fmaster%2Fsrc%2Fmodule.json&label=Latest%20Release&prefix=v&query=$.version&colorB=red&style=for-the-badge)

[![Foundry Hub Endorsements](https://img.shields.io/endpoint?logoColor=white&url=https%3A%2F%2Fwww.foundryvtt-hub.com%2Fwp-json%2Fhubapi%2Fv1%2Fpackage%2Fintroduce-me%2Fshield%2Fendorsements&style=for-the-badge)](https://www.foundryvtt-hub.com/package/introduce-me/)

![GitHub all releases](https://img.shields.io/github/downloads/p4535992/foundryvtt-introduce-me/total?style=for-the-badge)

[![Translation status](https://weblate.foundryvtt-hub.com/widgets/introduce-me/-/287x66-black.png)](https://weblate.foundryvtt-hub.com/engage/introduce-me/)

### if you feel generous you can to buy me a coffee [![alt-text](https://img.shields.io/badge/-Patreon-%23ff424d?style=for-the-badge)](https://www.patreon.com/p4535992)

A Foundry VTT module that lets you introduce NPCs or other actors to all players with some flair.

![](wiki/videos/introduce_me_preview.gif)

The fanfare will display the actor's name, and optionally a short flavor text that you can add to actors.
After the display, the actor will be set to display their name whenever someone hovers their token, since they have now been introduced!

# Usage

Actors can be introduced either via a button placed on the Token's HUD menu, accessed via right clicking it, or by using the macros included in the Introduce Me compendium. There is a module setting for disabling the HUD menu button if you're using the macros and don't want it taking space.

Flavor texts look best if they're not excessively long. The 'Private Preview' function can be used to check how it will look with the players none the wiser.

## Installation

It's always easiest to install modules from the in game add-on browser.

To install this module manually:
1.  Inside the Foundry "Configuration and Setup" screen, click "Add-on Modules"
2.  Click "Install Module"
3.  In the "Manifest URL" field, paste the following url:
`https://raw.githubusercontent.com/p4535992/foundryvtt-introduce-me/master/src/module.json`
4.  Click 'Install' and wait for installation to complete
5.  Don't forget to enable the module in game using the "Manage Module" button

### socketlib

This module uses the [socketlib](https://github.com/manuelVo/foundryvtt-socketlib) library for wrapping core methods. It is a hard dependency and it is recommended for the best experience and compatibility with other modules.

## Known issue

# API

The wiki for the API is [here](wiki/api.md)


# Build

## Install all packages

```bash
npm install
```

### dev

`dev` will let you develop you own code with hot reloading on the browser

```bash
npm run dev
```

### build

`build` will build and set up a symlink between `dist` and your `dataPath`.

```bash
npm run build
```

### build:watch

`build:watch` will build and watch for changes, rebuilding automatically.

```bash
npm run build:watch
```

### prettier-format

`prettier-format` launch the prettier plugin based on the configuration [here](./.prettierrc)

```bash
npm run-script prettier-format
```

### lint

`lint` launch the eslint process based on the configuration [here](./.eslintrc.json)

```bash
npm run-script lint
```

### lint:fix

`lint:fix` launch the eslint process with the fix argument

```bash
npm run-script lint:fix
```

### build:json

`build:json` unpack LevelDB pack on `src/packs` to the json db sources in `src/packs/_source`very useful for backup your items and manually fix some hard issue with some text editor

```bash
npm run-script build:json
```

### build:clean

`build:clean` clean packs json sources in `src/packs/_source`. NOTE: usually this command is launched after the command `build:json` and after make some modifications on the json source files with some text editor, but before the `build:db`

```bash
npm run-script build:clean
```

### build:db

`build:db` packs the json db sources in `src/packs/_source` to LevelDB pack on `src/packs` with the new jsons. NOTE: usually this command is launched after the command `build:json` and after make some modifications on the json source files with some text editor

```bash
npm run-script build:db
```

## [Changelog](./CHANGELOG.md)

## Issues

Any issues, bugs, or feature requests are always welcome to be reported directly to the [Issue Tracker](https://github.com/p4535992/foundryvtt-introduce-me/issues), or using the [Bug Reporter Module](https://foundryvtt.com/packages/bug-reporter/).

## License

- [Introduce Me](https://github.com/WBHarry/introduce-me) with [MIT](https://github.com/WBHarry/introduce-me/blob/main/LICENSE)

This package is under an [MIT license](LICENSE) and the [Foundry Virtual Tabletop Limited License Agreement for module development](https://foundryvtt.com/article/license/).

## Credit

- Thanks to [WBHarry](https://github.com/WBHarry) for the module [Introduce Me](https://github.com/WBHarry/introduce-me)
- Thanks to [DarKDinDoN](https://github.com/DarKDinDoN) for the module [Introduce Me (with some bug fix)](https://github.com/DarKDinDoN/introduce-me)
