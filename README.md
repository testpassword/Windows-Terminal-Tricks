# Setup ssh-profile

## 0. Preparing

Launch Windows Terminal, call the drop-down menu, and open the settings file. 

## 1. Creating profile

Create new profile with name, which your wanted and ssh profile in ```commandline``` attribute.

![Example of profile](img/ssh_example.png)

## 2. Adding an icon

Put image in some folder and add attribute ```icon``` to profile.

![Example of icon](img/icon_example.png)

Result:

![Result of ssh](img/res_ssh.png)

# Adding "Open Windows Terminal here" in context menu

## 0. Preparing

Clone the repository in any directory in your file system.

## 1. Setting the current directory as the default directory

Launch Windows Terminal, call the drop-down menu, and open the settings file. Add a key to the default profile settings: ```"startingDirectory": "."``` .
![Example settings.json](img/example.png)

This will tell the terminal to open in the current directory, not the home one.

## 2. Adding an item to the context menu

Run `` script.bat`` as administrator. In the end you get:
![Result of operation](img/result.png)

# Activating the new start menu in Windows 10 (not actual on Windows 10 2010)

![Comparison of old and new designs](example.gif)

## 0. Preparing

Go to ```Settings -> System -> About``` and check that you have version ```19041.423``` or above. If it's true, you can activate new menu.

## 1. Apply

Run [apply.reg](apply.reg) as administrator and restart explorer.exe or restart your computer to get new menu.

## 2. Undo

Run [undo.reg](undo.reg) as administrator and restart explorer.exe or restart your computer to return old menu.