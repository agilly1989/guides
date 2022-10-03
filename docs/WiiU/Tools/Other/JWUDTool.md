# JWUDTool

JWUDTool can be used to extract (decrypt) the WUP (or RAW) files from a WUD or WUX file

> [!NOTE]
> This is a command line/terminal tool, it has no GUI

## Downloads

* [GitHub :fas fa-up-right-from-square:](https://github.com/Maschell/JWUDTool)
    * [Release :fas fa-up-right-from-square:](https://github.com/Maschell/JWUDTool/releases/latest)


## Requirements

* Java
    * Install it from your repos or from [Eclipse Temurin :fas fa-up-right-from-square:](https://adoptium.net/temurin/releases/)


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
Compresses a WUD to a WUX
#### **`-decompress`**
Decompresses a WUX to a WUD
#### **`-decrypt`**
Decrypts the game partition of the input file to RAW files
#### **`-decryptFile REGEX`**
Decrypts the game partition of the input file to RAW files (Matching the Regex)
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

## ~~Command Builder~~ (Currently not working cause agilly doesn't know JavaScript)
Command: 
<pre v-pre="" data-lang=""><code class="lang-" name="command" id="command">java -jar Jnustool.jar</code></pre>

<!-- tabs:start -->
#### **Input File**
<input type="text" name="inputFile" value="INPUT WUD or WUX file/path"></input>

> [!Note]
> Use Double quotes `"` around your path if it has spaces

#### **WiiU Common Key**
<input type="radio" name="commonKey" value="" checked="true">`common.key` file</input><br>
<input type="radio" name="commonKey" value="-commonkey COMMONKEY">Manual entry <input type="text"></input></input><br>
#### **Disc Key**
<input type="radio" name="discKey" value="" checked="true">`game.key` file</input><br>
<input type="radio" name="discKey" value="-titleKey TITLEKEY">Manual entry <input type="text"></input></input><br>
<input type="radio" name="discKey" value="-dev">No key needed</input>
#### **Action**
<input type="radio" name="action" value="-decrypt" checked="true">Decrypt to RAW files</input><br>
<input type="radio" name="action" value="-decryptFile REGEX">Decrypt following the regex <input type="text" value=".*"></input></input><br>
<input type="radio" name="action" value="-extract OPTION">Extract ...
    <select name="extractOptions">
        <option value="all">All WUP files</option>
        <option value="content">All *.app files</option>
        <option value="ticket">All *.tik files</option>
        <option value="hashes">All *.h3 files</option>
    </select>
</input><br>
<input type="radio" name="action" value="-compress">Compress to a WUX</input><br>
<input type="radio" name="action" value="-decompress">Decompress to a WUD</input>

<!-- I don't know enough JS to make this work... PLZ HALP -->

<!-- tabs:end -->