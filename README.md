# Install Ubuntu 15

![alt text](http://core0.staticworld.net/images/article/2014/08/logo-ubuntu-100372440-primary.idge.png "Ubuntu 15.10")

#Performing a Clean Install of Ubuntu 15.10

**Total Estimated time: 30-45 minutes**

**Required items:**

USB drive with at least 6GB of storage

**Index:**

1. Backing up Files and Settings
2. Mounting Ubuntu on a USB drive
3. Installing Ubuntu
4. Additional software

#1. Backing up Files and Settings

1. Click on the Start Menu > All Programs > Accessories > System Tools backup.
2. Click next and select the Back up files and settings.
3. Select what to backup from the options listed.
4. Choose where to back up the files and name it.
*Note: back up sizes will vary.* 


#2. Mounting Ubuntu on a USB drive

1. Download the appropriate Ubuntu file and place it on your desktop.

    [32-bit](http://www.ubuntu.com/download/desktop/thank-you/?version=15.10&architecture=i386) (2GB RAM or less)
    
    [64-bit](http://www.ubuntu.com/download/desktop/thank-you/?version=15.10&architecture=amd64) (Recommended)
    
2. Click [here](http://www.pendrivelinux.com/downloads/Universal-USB-Installer/Universal-USB-Installer-1.9.6.3.exe) to install a Universal USB Installer and move it to your desktop.
3. Run the USB installer and select Ubuntu from the first dropdown menu.
4. Select the Ubuntu .iso file you had saved from earlier.
5. Select the flash drive you will be using to install Ubuntu and click the create button.
6. Wait for the file to extract to the USB drive.
7. Safely eject the USB drive from your task bar and plug the USB drive into the machine you will be installing Ubuntu on.


#3. Installing Ubuntu

1. Insert the USB drive into the computer that you will be installing Ubuntu on.
2. Restart the computer. As soon as the first text appears on the screen, press the appropriate button to enter your BIOS/system setup which is usually one of the following keys: F1, F2, Del, Esc, F10, F11, or F12.
3. Once in the BIOS change the option for boot sequence to boot from the USB drive you installed Ubunutu on.
4. Once the boot order is changed restart your computer.
5. Wait a minute or two, an install window will appear.
6. Select English from the list to the left of the screen and click Install Ubuntu.
7. Follow the instructions on the screen to select your country, timezone and keyboard layout.
8. When you get to the Prepare disk space screen, choose which option best suits your needs, I chose to erase Windows XP completely.
9. Follow the instructions to choose a username and password.
10. Click Install. The installation will begin, and should take 10-20 minutes to complete. When it is finished, choose to restart the computer and then remove your memory stick. Ubuntu should start to load.

#4. Additional Software

###Chromium
Chromium is an open-source version of Chrome. 

1. Change to root directory:

    ```bash
$ cd ~
```

2. Add the Chromium PPA:
    
    ```bash
$ add-apt-repository ppa:chromium-daily/ppa
```

3. Download the package lists from the repositories and "update" them to get information on the newest versions of packages and their dependencies. It will do this for all repositories and PPAs.

    ```bash
$ sudo apt-get update
```

4. Install Chromium:
    
    ```bash
$ sudo apt-get install chromium-browser
```

###Sublime Text 3
Sublime Text is a sophisticated text editor for code, html and prose. 

1. Change to root directory:

    ```bash
$ cd ~
```

2. Add the WebUpd8 Sublime Text 3 (beta) PPA:
    
    ```bash
$ sudo add-apt-repository ppa:webupd8team/sublime-text-3
```

3. Download the package lists from the repositories and "update" them to get information on the newest versions of packages and their dependencies. It will do this for all repositories and PPAs.

    ```bash
$ sudo apt-get update
```

4. Install Sublime Text 3:
    
    ```bash
$ sudo apt-get install sublime-text-installer
```

5. Add in drupal specific preferences [https://drupal.org/node/1346890](https://drupal.org/node/1346890)

###IRC (HexChat)
1. Add the HexChat PPA:
    
    ```Bash
$ sudo add-apt-repository ppa:gwendal-lebihan-dev/hexchat-stable
```

2. Download the package lists from the repositories and "update" them to get information on the newest versions of packages and their dependencies. It will do this for all repositories and PPAs
    
    ```Bash
$ sudo apt-get update
```

3. Install HexChat:
    
    ```Bash
$ sudo apt-get install hexchat
```

###Terminator

1. Change to root directory:

    ```bash
$ cd ~
```

2. Add the Terminator Nightly Builds PPA:
    
    ```bash
$ sudo add-apt-repository ppa:gnome-terminator/nightly
```

3. Download the package lists from the repositories and "update" them to get information on the newest versions of packages and their dependencies. It will do this for all repositories and PPAs.

    ```bash
$ sudo apt-get update
```

4. Install Terminator:
    
    ```bash
$ sudo apt-get install terminator
```



