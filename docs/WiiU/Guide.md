# Getting Titles onto a WiiU or Cemu

> [!NOTE]
> This guide will not host pirated content, it is used for informational purposes only

## Terminology and info before you start

<!-- tabs:start -->

#### **Title File Formats**

* [WUD](/WiiU/Formats/WUDX)
    * WiiU Disc Image
* [WUX](/WiiU/Formats/WUDX)
    * Compressed WiiU Disc Image
* [WUP](/WiiU/Formats/WUP)
    * WiiU Package
* [RAW](/WiiU/Formats/RAW)
    * This is the "[RAW](WiiU/Formats/RAW)" files, otherwise known as "Code, Content and Meta" or "Loadiine"
* [WUA :fas fa-up-right-from-square:](https://github.com/Exzap/ZArchive)
    * WiiU Archive (at the time of writing, this guide won't cover the usage of WUA)

#### **Homebrew File Formats**

<!--- Need to update later --> 

* ELF
    * An outdated WiiU homebrew format
* RPX
    * A WiiU homebrew format
    * Can be used on all CFWs
* WUHB
    * WiiU Homebrew Bundle
    * Aroma Only

#### **Actions**

* Unpack
    * The decryption of the [RAW](WiiU/Formats/RAW) files from the [WUD](WiiU/Formats/WUDX)/[WUX](WiiU/Formats/WUDX) or [WUP](WiiU/Formats/WUP)
* Pack
    * The encryption of a [WUP](WiiU/Formats/WUP) from [RAW](WiiU/Formats/RAW) files
* Download
    * The action of getting a program to download a file from the internet
* Install
    * The action of installing a title to your WiiU or to an Emulator
* Running
    * The action of opening software and running it

#### **Misconceptions**

* You can make a [WUD](WiiU/Formats/WUDX)/[WUX](WiiU/Formats/WUDX)
    * At the time of writing, the only way you can make a [WUD](WiiU/Formats/WUDX) or a [WUX](WiiU/Formats/WUDX) is dumping one from an actual disc on a WiiU
* A [WUX](WiiU/Formats/WUDX) is smaller than [RAW](WiiU/Formats/RAW) files
    * This is incorrect... See [this information :fas fa-up-right-from-square:](https://www.reddit.com/r/CemuPiracy/comments/g08qxj/some_research_i_have_been_doing_into_game_sizes/)

#### **Other Terms**

* Disc Key
    * This is the key that is used to decrypt the Disc (Image) ([WUD](WiiU/Formats/WUDX)/[WUD](WiiU/Formats/WUDX))
* Title Key
    * This is the key that is used to decrypt the [WUP](WiiU/Formats/WUP)
* Common Key
    * This key is common to all WiiUs and can easily be found by Google
        * Search for `WiiU Common Key D7` and you will find a 32 character long key that starts with `D7B` and ends with `656`
* Ancast Key
    * Used for cafe2wii things (like unlocking the vWii clock limiter)
        * Search for `WiiU Ancast Key B5` and you will find a 32 character long key that starts with `B5D` and ends with `2FD`
* NUSDownloader
    * A tool that can download from the NUS
* NUS
    * Nintendo Update Servers, Where all the E-shop games are stored (basically)
* Injection
    * A "clone" of a Virtual Console title that has been fooled into running a different game


<!-- tabs:end -->

## What are you installing the title too?

<!-- tabs:start -->

#### **WiiU**

[Nintendo Homebrew WiiU modding guide :fas fa-up-right-from-square:](https://wiiu.hacks.guide)

You are currently limited to installing/running 2 formats on the WiiU

* [WUP](/WiiU/Formats/WUP) (Recommended)
* [RAW](/WiiU/Formats/RAW) (via Loadiine, Not recommended at all)

#### **Cemu**

[Official Cemu guide :fas fa-up-right-from-square:](https://cemu.cfw.guide)

Cemu can open a range of formats

* [WUD](/WiiU/Formats/WUDX)
* [WUX](/WiiU/Formats/WUDX)
* [RAW](/WiiU/Formats/RAW) (Recommended)
* [WUA :fas fa-up-right-from-square:](https://github.com/Exzap/ZArchive)

> [!NOTE]
> Please note: [WUD](WiiU/Formats/WUDX) and [WUX](WiiU/Formats/WUDX) require the correct **DISC** key (not the **TITLE** key) and possibly the WiiU Common Key in the `keys.txt` file that can be put next to `cemu.exe`

<!-- tabs:end -->