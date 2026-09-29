# CommonLibSSE-NG Plugin Template

This is a basic plugin template using CommonLibSSE-NG.

### Requirements
* [XMake](https://xmake.io) [2.8.2+]
* C++23 Compiler (MSVC, Clang-CL)

## Getting Started
```bat
git clone MYGITHUBURL commonlibsse-ng-template
cd commonlibsse-ng-template
git submodule add https://github.com/alandtse/CommonLibSSE-NG.git lib/commonlibsse-ng
git submodule update --init --recursive
```

### Change project name and author in xmake.lua

### Update commonlibng : 
```
cd lib/commonlibsse-ng
git fetch --tags
git checkout main
git pull origin main
```

### Build
To build the vs project, run the following command:
```bat
xmake project -k vsxmake
```

### Build Output (Optional)

#### Mod Directory
Set one of or both of the following environment variables:

- Path to a Skyrim install folder: `XSE_TES5_GAME_PATH`

- Path to a Mod Manager mods folder: `XSE_TES5_MODS_PATH`

#### Mod Resources
Copy resources like ini files, Bethesda plugins, etc. with the custom rule `copy_resource`
