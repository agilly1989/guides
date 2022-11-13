# JNUSTool

## Links
* [GitHub :fas fa-up-right-from-square:](https://github.com/Maschell/JNUSTool)
    * [Release :fas fa-up-right-from-square:](https://github.com/Maschell/JNUSTool/releases/latest)


## Output Formats

* [WUP](/WiiU/Formats/WUP) (No `title.tik` unless one exists on the NUS)
* [RAW](/WiiU/Formats/RAW) (If supplied with a Title Key and the WiiU Common Key)

## Requirements

* Java
    * Install it from your repos or from [Eclipse Temurin :fas fa-up-right-from-square:](https://adoptium.net/temurin/releases/)

## Pros and Cons

<!-- tabs:start -->

#### **Pros**

### Pros

* Speed
* Cross Platform

#### **Cons**

### Cons

* *Can* be too fast for its own good and may crash/finish before finishing
    * Solution: Run the command multiple times till it is "done"
        * Make a script to loop over the command "quite a few times" and then wait
        * It will skip files that are complete by checking sizes and hashes

#### **Other**

### Other

* Has a GUI but can only be used for Title Updates

<!-- tabs:end -->

## Usage

Before anything...

Open `config` in a text editor and replace the `[COMMONKEY]` line with the WiiU Common Key (No spaces or dashes)

<!-- tabs:start -->
#### **Command Line/Terminal**

### Command Line/Terminal

Follow this part from top to bottom, each argument is the tab name so for example

* `java -jar Jnustool.jar TitleID -dlEncrypted`
* `java -jar Jnustool.jar TitleID TitleKey -file .* v208`


<!-- tabs:start -->
#### **`java -jar Jnustool.jar`**
Make sure the jar you downloaded and the one in the command is the same name
<!-- tabs:start -->
#### **`TitleID`**
Enter the Title ID without any spaces or dashes

Can be located at the following
* [WiiUBrew Title Database :fas fa-up-right-from-square:](https://wiiubrew.org/wiki/Title_database)
* [vault.titlekeys.ovh :fas fa-up-right-from-square:](http://vault.titlekeys.ovh/listing/)
* [agillys title key page :fas fa-up-right-from-square:](https://wiiu.agilly1989.xyz/keylist.htm)

<!-- tabs:start -->
#### **`TitleKey`**
Only needed if you want to Decrypt to [RAW](WiiU/Formats/RAW)

Can be located at the following
* [vault.titlekeys.ovh :fas fa-up-right-from-square:](http://vault.titlekeys.ovh/listing/)
* [agillys title key page :fas fa-up-right-from-square:](https://wiiu.agilly1989.xyz/keylist.htm)

<!-- tabs:end -->

<!-- tabs:start -->
#### **`-dlEncrypted`**

Downloads a [WUP](WiiU/Formats/WUP)

#### **`-file REGEX`**

Download [RAW](WiiU/Formats/RAW) files that match the `REGEX` pattern. Recommended `REGEX` is `.*`

> [!Note]
> You may need to use your distros/terminals escape characters for it to work properly

> [!Warning]
> `TitleKey` is required

<!-- tabs:end -->

<!-- tabs:start -->

#### **`vXXX`**

OPTIONAL, Will download the latest if ommitted

Download a specific version. Replace the XXX with the *internal* version of the title

<!-- tabs:end -->
<!-- tabs:end -->
<!-- tabs:end -->

#### **GUI**
### GUI

To be completed

<!-- tabs:end -->