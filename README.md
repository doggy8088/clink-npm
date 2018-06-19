# clink-npm

This repo contains a [Lua](https://www.lua.org) script for [npm CLI](https://docs.npmjs.com) completion used in [Clink](https://mridgers.github.io/clink/).

## Install

1. Install [Clink](https://mridgers.github.io/clink/) first
    * `choco install clink2 -y`
    * The default installation path should be at `%ProgramFiles(x86)%\clink\0.4.9`.
2. Edit `%ProgramFiles(x86)%\clink\0.4.9\clink.lua` file
    * Copy all content of the `npm.lua` to the bottom of the `clink.lua` file.

## Usage

* `npm <TAB><TAB>`
  * This will show all the available NPM CLI commands.
* `npm ru<TAB>` --> `npm run-script <TAB><TAB>`
  * This will show all the available **scripts** in the `package.json` of current folder.

## Credits

* The embedded Lua JSON parser in the `npm.lua` is comes from [Jeffrey Friedl's Blog » Simple JSON Encode/Decode in Pure Lua](http://regex.info/blog/lua/json).
