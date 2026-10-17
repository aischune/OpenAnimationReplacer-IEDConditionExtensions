# OpenAnimationReplacer-IEDConditionExtensions

This is a SKSE64 plugin that lets OAR read data from IED and SDS via conditions.

Current release target runtime: **Skyrim SE/AE 1.7.104**.

### Requirements
* [XMake](https://xmake.io) [2.7.8+]
* C++20 Compiler (MSVC, Clang?)

## Getting Started
```bat
git clone https://github.com/SlavicPotato/OpenAnimationReplacer-IEDConditionExtensions
cd OpenAnimationReplacer-IEDConditionExtensions
```

### Build
To build the project, run the following command:
```bat
xmake build
```

To build for Skyrim VR instead:
```bat
xmake f --skyrim_vr=y
xmake build
```

> ***Note:*** *This will generate a `build/windows/` directory in the **project's root directory** with the build output.*

### Build Output (Optional)
If you want to redirect the build output, set one of or both of the following environment variables:

- Path(s) to a Skyrim install folder: `SKYRIM_PATH`

- Path(s) to a Mod Manager mods folder: `SKYRIM_MODS_PATH`

> ***Note:*** *Both variables support semicolon (`;`) seperated paths for multiple game installs or `mods` folders.*

### Project Generation (Optional)
If you want to generate a Visual Studio project, run the following command:
```bat
xmake project -k vsxmake
```

> ***Note:*** *This will generate a `vsxmakeXXXX/` directory in the **project's root directory** using the latest version of Visual Studio installed on the system.*

### Upgrading Packages (Optional)
If you want to upgrade the project's dependencies, run the following commands:
```bat
xmake repo --update
xmake require --upgrade
```

## Release Notes
- **1.0.2**: Added explicit Skyrim SE/AE 1.7.104 target runtime support in build configuration, with optional VR build toggle.
