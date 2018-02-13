Jade
====

Jade is an Alternative Development Environment (IDE) for GemStone/S that runs on Microsoft Windows. This [screencast](https://www.youtube.com/watch?v=dnRB5rBbkiI) gives a brief demo from 2013. 

Jade is built in (and inspired by) Dolphin Smalltalk from [Object-Arts](https://github.com/dolphinsmalltalk/Dolphin).

### Runtime Installation
To install Jade runtime, download a 35 MB zip file with the executable and supporting libraries from [here](https://github.com/jgfoster/Jade/raw/master/runtime/Jade.zip). Once you have the environment, you can get just the latest executable (about 1.5 MB) from [here](https://github.com/jgfoster/Jade/raw/master/runtime/Jade.exe).

Older versions are available using the instructions [here](https://github.com/jgfoster/Jade/issues/56).

Jade runs pretty well under [Wine](https://www.winehq.org/) and a pre-built Mac app is available [here](http://seaside.gemtalksystems.com/jade/Jade.app.zip). It may be out-of-date, so you can use “Show Package Contents” and then update "drive_c/Program Files/Jade” with items obtained from [here](https://github.com/jgfoster/Jade/raw/master/runtime/Jade.zip).

### Development Installation

To install Martin's fork of Jade in Dolphin 7, follow these steps:

1. Install a Git client such as [SourceTree](http://www.sourcetreeapp.com/).
2. Pick a place to put your local repositories and builds. I will call this place \Dolphin.
3. Clone [Dolphin](https://github.com/martinmcclure/Dolphin) to \Dolphin.
4. Clone [DolphinVM](https://github.com/martinmcclure/DolphinVM) to \Dolphin\DolphinVM.
5. Follow the instructions in \Dolphin\DolphinVM\README.md to build the Dolphin VM using VisualStudio 2017.
6. Run \Dolphin\BootDPRO.cmd to build the base Dolphin pro image, DPRO.img7.
7. Clone [Jade](https://github.com/martinmcclure/Jade) to\Dolphin\Jade. (You can make this a Git subproject if you're comfortable with Git.)
8. Run \Dolphin\Jade\BootJade.cmd to build the JadeDev image.
9. Finally, from the Additional Tools folder in the System Shell open the Jade Login.
