# WUD and WUX

To get a WUD or WUX file, you can use whatever method you choose

> [!NOTE]
> Remeber, a WUD is a full disc image so it will be about 25GB in size. If you do not need a WUD or a WUX avoid downloading it. To confirm if you need it or not, check the [WiiUBrew title database "eShop and disc titles" section :fas fa-up-right-from-square:](https://wiiubrew.org/wiki/Title_database#00050000:_eShop_and_disc_titles) and if it says "No TMD" it is either Disc Only or is no longer available from the NUS

<!-- tabs:start -->

#### **From A Disc**

## From A Disc

You can use `wudd`
* [Github :fas fa-up-right-from-square:](https://github.com/wiiu-env/wudd)
    * [Latest Release (could be wuhb only) :fas fa-up-right-from-square:](https://github.com/wiiu-env/wudd/releases/latest)
    * [Appstore ver (has an rpx release) :fas fa-up-right-from-square:](https://github.com/wiiu-env/wudd/releases/tag/v1.2.1)
    * Should be able to be found on the WiiU Homebrew Appstore as well

<!-- tabs:start -->

#### **Onto a WiiU**

### Onto a WiiU

See [WiiU Guide: Dumping WiiU Discs :fas fa-up-right-from-square:](https://wiiu.hacks.guide/#/dump-games)

#### **Onto Cemu**

### Onto Cemu

* Converting to [RAW](/WiiU/Formats/RAW) (Recommended)
* Adding key to `keys.txt` and running WUD/WUX (Not really recommended but people do it anyway)
    * Open (with a hex editor) the `game.key` file provided by `wudd` and add the key found (16 hex characters) without spaces to the `keys.txt` file next to `cemu.exe`
        * Recommended Hex editor for Windows: [HXD :fas fa-up-right-from-square:](https://mh-nexus.de/en/hxd/)

<!-- tabs:end -->

#### **From Not A Disc**

## From Not A Disc

Then Google/Bing/DuckDuckGo is your friend... But to help you start, some search terms can be
* WiiU WUD download
* WiiU WUX download
* [r/roms :fas fa-up-right-from-square:](https://www.reddit.com/r/Roms/) megathread
* Rom To Home
* WiiU alvro
* [game name] WUD / WUX

<!-- tabs:start -->

#### **Onto a WiiU**

### Onto a WiiU

Convert to a [WUP](/WiiU/Formats/WUP)

#### **Onto Cemu**

### Onto Cemu

* Converting to [RAW](/WiiU/Formats/RAW) (Recommended)
* Adding key to `keys.txt` and running WUD/WUX (Not really recommended but people do it anyway)
    * Open (with a hex editor) the `game.key` file provided by `wudd` and add the key found (16 hex characters) without spaces to the `keys.txt` file next to `cemu.exe`
        * Recommended Hex editor for Windows: [HXD :fas fa-up-right-from-square:](https://mh-nexus.de/en/hxd/)
    * If there is no `game.key` file, the key might be provided somewhere else with the download...
        * On the download page itself
        * In a `.nfo` file
        * In a `.bin` file
        * etc

<!-- tabs:end -->

<!-- tabs:end -->

