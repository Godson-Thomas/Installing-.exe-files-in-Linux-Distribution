## Installing Wine on Ubuntu 18.04 
# WINE
<img src="https://github.com/Godson-Thomas/Installing-.exe-files-in-Linux-Distribution/blob/master/Images/1_Wine.jpeg" width="400">  <br>
Wine is a free and open source software application that aims to allow computer programs written for Microsoft Windows to run on Unix-like operating systems. Wine also provides a software library, known as Winelib, against which developers can compile Windows applications to help port them to Unix-like systems.
### Note : We are going to install Wine 3.0.However, the version included  may lag behind the latest version of Wine.


# Installation
1. Open your Terminal by pressing **Ctrl+Alt+T**<br><br>
<img src="https://github.com/Godson-Thomas/Installing-.exe-files-in-Linux-Distribution/blob/master/Images/2_terminal.png" width="500">  <br><br>
2. Start by enabling the 32-bit architecture.
```
sudo dpkg --add-architecture i386
```
3. Update your Packages.
```
sudo apt-get update
```
4. Use this command to display your Architecture model
```
lscpu
```
### Note :<br>
if you are running a 64-bit Ubuntu system, you have to install both 64 and 32-bit packages on the same machine. This is because most of the Windows applications runs on 32-bit architecture.

5. Install Wine.<br>

```
sudo apt install wine64 wine32
```
6. use this command to check your wine version.
```
wine --version
```
The Wine version will be displayed if the packages are installed correctly.
# Wine 3.0 Configuration
7. Open Wine from terminal by typing
```
winecfg
```
<img src="https://github.com/Godson-Thomas/Installing-.exe-files-in-Linux-Distribution/blob/master/Images/3_Wine_cfg.png" width="400">  <br><br>
8.You can select your Windows Version.
# Installing a Windows Executable(.exe) file
## Installation of Notepad++
9. Download the Notepad++ installer file from [here](https://notepad-plus-plus.org/downloads/).
10. Go to the folder where you have downloaded the **.exe** file<br><br>
<img src="https://github.com/Godson-Thomas/Installing-.exe-files-in-Linux-Distribution/blob/master/Images/4_Folder.png" width="400">  <br><br>
11. **Right Click** >> **Open in Terminal**
12. Type
```
wine Your_installer_name.exe
```
13. The installer will be opened.Now complete the installation process.<br><br>
<img src="https://github.com/Godson-Thomas/Installing-.exe-files-in-Linux-Distribution/blob/master/Images/5_Note.png" width="400">  <br><br>

14. After the installation you can open **Notepad++** from the **Show Applications** tab on your desktop.