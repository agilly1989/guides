# WUP (WiiU Package)

A WUP can be identified by a set of files that look like this

```
📁 gamename_folder
┣ title.tmd
┣ title.tik
┣ title.cert
┣ *.app
┗ *.h3
```

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

<!-- tabs:start -->

#### **From a WUD/WUX File**

### From a WUD/WUX File

1. See [WUD/WUX](/WiiU/Formats/WUDX?id=from-not-a-disc) to get a WUD or WUX file
2. Use one of the following tools to unpack the WUP from the disc image
* [JWUDTool](/WiiU/Tools/Other/JWUDTool)

#### **From RAW**

### From RAW

* [NUSPACKER :fas fa-up-right-from-square:](https://github.com/ihaveamac/nuspacker) (Java)
    * If you don't have java, install it from your repos or from [Eclipse Temurin :fas fa-up-right-from-square:](https://adoptium.net/temurin/releases/)
* [CNUSPACKER :fas fa-up-right-from-square:](https://github.com/NicoAICP/CNUS_Packer) (C# port of NUSPACKER)

> [!WARNING]
> You can not pack title updates as there are special files that symlink/hardlink to files that exist in the game itself. If you wish to pack an update, you will need to get the game and update as [RAW](/WiiU/Formats/RAW) and Copy the Games `content` folder onto the updates `content` folder **NOT** overwriting files

#### **From NUS**

### From NUS

* Use a [NUSDownloader](/WiiU/Tools/Nusdownloader) (Recommended)
* [Download it manually](/Masochism/NUSDownload) (Highly not recommended)

<!-- tabs:end -->

At this point you should have a WUP

<!-- tabs:start -->

#### **Onto A WiiU**

### Onto A WiiU

1. Copy the WUP to `sd:/install/gamename_folder` so it looks like this

```
💾 SD card root
┗ 📁 install
   ┗ 📁 gamename_folder
      ┣ title.tmd
      ┣ title.tik
      ┣ title.cert
      ┣ *.app
      ┗ *.h3
```

> [!NOTE]
> * `install` must be lowercase
> * `gamename_folder` must be only ascii characters, no special characters at all

2. Get WUP Installer GX2 from the Homebrew Appstore
3. Install the WUP(s)


#### **Onto Cemu**

### Onto Cemu

Unpack the WUP into RAW files with a tool below
* [JNUSLib Decryptor :fas fa-up-right-from-square:](https://github.com/Maschell/JNUSLibDecryptor) (Java)
    * If you don't have java, install it from your repos or from [Eclipse Temurin :fas fa-up-right-from-square:](https://adoptium.net/temurin/releases/)
* CDecrypt
    * [Version 2.0b :fas fa-up-right-from-square:](https://gbatemp.net/download/cdecrypt.35671/)
    * [Version 3.0 :fas fa-up-right-from-square:](https://gbatemp.net/threads/release-cdecrypt-v3-0.554220/)
    * [Version 4.x :fas fa-up-right-from-square:](https://gbatemp.net/threads/release-cdecrypt-v4-x.578790/)
    * etc (Fix this later lol)

And then ["install" into Cemu :fas fa-up-right-from-square:](https://cemu.cfw.guide/installing-games.html?tab=installing-dumps#saves)

<!-- tabs:end -->

<!-- tabs:end -->