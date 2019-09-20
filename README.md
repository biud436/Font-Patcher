# Introduction
The Font Patcher is a great tool that can change the game font without editing the game is developed by using RPG Maker VX Ace.

[![FontPatcher](https://img.youtube.com/vi/yo0uyegrvo8/0.jpg)](https://youtu.be/yo0uyegrvo8)

# Download
This tool is possible to change the font face of the game that has been made using RPG Maker VX Ace.

EXE : https://github.com/biud436/RGSS3/raw/master/FontPatcher/bin/FontPatcher.exe

DLL : https://github.com/biud436/RGSS3/raw/master/FontPatcher/bin/RSFont.dll


# Sources

Font Patcher (EXE) : https://github.com/biud436/Font-Patcher
RGSSFont (DLL) : https://github.com/biud436/RGSSFont

# Setup

- You should place both of RSFont.dll and FontPatcher.exe files in the Root Game Directory that has the file called 'Game.exe'
- Please try to run the game using FontPatcher.exe file. As a result, the game will be going to change the font. However, In case of clicking the default executable file called 'Game.exe' directly, it doesn't change the font.
- This font changer doesn't read font files in the project's Fonts folder, so you should add a font file to Windows' Fonts folder you want and install the font. 

# Features

- A Decryption of the encrypted game resources is illegal, so this tool does not rewrite script files and it will be going to change the default font and font size by injecting the 'RSFont.dll' file during the runtime. so the changed font is not permanent.
- The one core principle of changing the font is to override the class variables named 'Font.default_name' and 'Font.default_size' and some constants. but actually, some fonts may not be changed.
- This has been implemented a way to inject the DLL file directly into the target process(Game.exe), so the anti-virus program may diagnose it as the malware. But it is not malware.
- it is only tested in Windows 10.
- You could use any font that is in the Windows' Fonts folder excluding the System Font is already using.

# Version Log

```
2019.09.16 (v1.0.0) : First Release.
2019.09.17 (v1.0.1) : 
- Fixed the issue that is not changed with the Korean Font.
- Fixed the issue that is caused by incorrect use of CreateProcess function.
- The UI has been changed from console-based to GUI-based.
2019.09.18 (v1.0.2) :
- Now Yanfly Ace Message System is supported.
2019.09.20 (v1.0.3) :
- Added the new feature that can store the last index of the combo-box..
- Changed the UI color and Added the static control.
```