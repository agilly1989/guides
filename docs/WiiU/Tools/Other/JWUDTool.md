# JWUDTool

JWUDTool can be used to extract (decrypt) the [WUP](WiiU/Formats/WUP) (or RAW) files from a [WUD](WiiU/Formats/WUDX) or [WUX](WiiU/Formats/WUDX) file

> [!NOTE]
> This is a command line/terminal tool, it has no GUI

## Downloads

[GitHub :fas fa-up-right-from-square:](https://github.com/Maschell/JWUDTool) -- [Release :fas fa-up-right-from-square:](https://github.com/Maschell/JWUDTool/releases/latest)


## Requirements

Java -- [Eclipse Temurin :fas fa-up-right-from-square:](https://adoptium.net/temurin/releases/)


## Usage

<!-- tabs:start -->
#### **Command Line/Terminal**

### Command Line/Terminal

Follow this part from top to bottom, each argument is the tab name so for example ...

<!-- tabs:start -->

#### **`java -jar jwudtool.jar`**

Change the filename either in the command or the file itself so it can be used

<!-- tabs:start -->
#### **`-in InputFile`**
Required - can be
* `.wud`
* `.wux`
* `*_part1.wud`

<!-- tabs:end -->

<!-- tabs:start -->
#### **`-commonkey WiiU_Commonkey`**
Optional BUT if you dont use it, you will need a `common.key` file in the same folder as the `.jar` file
<!-- tabs:end -->

<!-- tabs:start -->

#### **`-titleKey DiscKey`**
Optional BUT if you dont use it, you will need a `game.key` file in the same folder as the `.WUD`/`.WUX` file
#### **`-dev`**
Used for discs that don't have a "Title Key" (Disc Key)

<!-- tabs:end -->

<!-- tabs:start -->
#### **`-compress`**
Compresses a [WUD](WiiU/Formats/WUDX) to a [WUX](WiiU/Formats/WUDX)
#### **`-decompress`**
Decompresses a [WUX](WiiU/Formats/WUDX) to a [WUD](WiiU/Formats/WUDX)
#### **`-decrypt`**
Decrypts the game partition of the input file to [RAW](WiiU/Formats/RAW) files
#### **`-decryptFile REGEX`**
Decrypts the game partition of the input file to [RAW](WiiU/Formats/RAW) files (Matching the Regex)
#### **`-extract OPTION`**
Extracts the following (replace `OPTION` with what you want)
* `all` = All files related to a WUP
* `content` = All `*.app` files (need to confirm)
* `ticket` = All `*.tik*` files (need to confirm)
* `hashes` = All `*.h3*` files (need to confirm)
<!-- tabs:end -->

<!-- tabs:start -->
#### **`-out OutPath`**
Required - This is your output path

<!-- tabs:end -->

<!-- tabs:end -->
<!-- tabs:end -->