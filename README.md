# Sonic Hybrid RSDK

Aims to mix different Sonic the Hedgehog games into a single big game.

![Sonic 1 in Sonic 2](docs/preview.png)

## Start from here

This guide is useful if you never downloaded the project or if you want to start from scratch.

1. [Download](https://github.com/Xeeynamo/sonic-hybrid-rsdk/archive/refs/heads/main.zip) the latest release

1. Unpack the zip file

1. Paste in the directory `rsdk-source-data` the following files:

    * `Data.rsdk` from Sonic CD as `soniccd.rsdk`
    * `Data.rsdk` from Sonic 1 as `sonic1.rsdk`
    * `Data.rsdk` from Sonic 2 as `sonic2.rsdk`

1. Install [.NET 6](https://dotnet.microsoft.com/download/dotnet/6.0)

1. Open a terminal and run the command `dotnet run --project SonicHybridRsdk.Build`

1. Put the [RSDKv4](https://github.com/Rubberduckycooly/Sonic-1-2-2013-Decompilation/releases) engine in the `sonic-hybrid` folder

1. Run the RSDKv4 executable and have fun!

## Perform an update

This guide is useful if you previously played Sonic Hybrid but you want to perform an update.

1. [Download](https://github.com/Xeeynamo/sonic-hybrid-rsdk/archive/refs/heads/main.zip) the latest release

1. Unpack the zip file and overwrite all the existing files

1. Open a terminal and run the command `dotnet run --project SonicHybridRsdk.Build`

1. Run the RSDKv4 executable and have fun!

## Features

* Star Posts in Sonic the Hedgehog 1 will bring you to the Sonic the Hedgehog 2 special stages.
* Completing Sonic the Hedgehog 1's Final Zone will bring you to Emerald Hill Zone.
* The Stage Select in the debug menu will report all the implemented level names.

## Known bugs

* Special Stages from the Giant Ring in Sonic the Hedgehog 1 are not working.
* Giant Ring graphics from Sonic 1 is currently broken.
* Sonic 1 Special Stages are working from the Stage Select, but the graphics is corrupted.
* Loops in Sonic the Hedgehog 1 are currently broken.
* The main menu of RSDK will report the wrong stage names.
* The title card for Sonic the Hedgehog 1 levels will not display the act number correctly.

## Resources

Everything contained in `rsdk/Scripts` is a modified version of [Rubberduckycooly's Sonic 1/2 script decompilation](https://github.com/Rubberduckycooly/Sonic-1-Sonic-2-2013-Script-Decompilation). This project would not exist without it.

The function `SonicHybridRsdk.Unpack12/DecryptData` was written by Giuseppe Gatta (nextvolume) from its [Retrun](http://unhaut.epizy.com/retrun/).
