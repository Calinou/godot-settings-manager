# Godot Settings Manager

An autoload to make settings management easier.

## Features

- Manage multiple configuration files easily.
  - For instance, to make it easier for users to backup their settings,
    you can have one "user" settings file containing user preferences,
    one "system" settings file containing system-dependent settings
    and a "cache" settings file with temporary values that can be
    safely deleted.
- Centralized storage for default values in the Project Settings.
  - No more duplication if you need to use the same setting in several places.
- Smart, resilient saving.
  - Saves settings automatically when quitting.
  - Saves settings if a setting was changed recently, with a short debounce
    delay to avoid unnecessary I/O. This way, settings are preserved if the
    project crashes.

## Demo

See [godot-settings-manager-demo](https://github.com/Calinou/godot-settings-manager-demo).

## Installation

**This asset currently requires
[Godot 3.1 alpha 4](https://godotengine.org/article/dev-snapshot-godot-3-1-alpha-4)
or later.**

- Clone this repository or
  [download a ZIP archive](https://github.com/Calinou/godot-settings-manager/archive/master.zip).
- Add `addons/settings_manager/settings_manager.gd` as an autoload in your project's settings.
  You can give it any name you wish, but it's recommended to use `SettingsManager`
  as a convention.

## License

Copyright © 2018 Hugo Locurcio and contributors

Unless otherwise specified, files in this repository are licensed under
the MIT license; see [LICENSE.md](LICENSE.md) for more information.
