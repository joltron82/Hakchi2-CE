[General](./page2.md)
[Supported devices](./page2.md)
[hakchi2-CE UI](./page2.md)
# HAKCHI FAQ
***
***

## General 
***
#### What is hakchi

hakchi2 CE is a modification program for Retro gaming consoles that provides the ability to add additional games and content to the console. 
Examples include
Nintendo: NES, SNES, Famicom, Super Famicom
Sega: Genesis, Mega Drive

#### Notes on previous versions
hakchi, hakchi2 and hakchi2-CE are 3 separate entities.

hakchi is the modification installed on mini systems that gives you the ability to add additional games and content to your system.
hakchi was created by madmonkey and has received contributions from numerous contributors. 

hakchi2 is the frontend for hakchi, hakchi2 was originally created by clusterm and has since been forked into hakchi2 CE which is maintained by Team Shinkansen.

hakchi2 CE by Team Shinkansen is the preferred tool for managing and installing hakchi onto consoles.

Throughout this document hakchi is used in general for both hakchi and hackhi2 CE
 

#### Where can I download it?
hakchi2 CE can be found from the Team Shinkansen releases page on GitHub.

http://github.com/teamshinkansen/hakchi2-ce/releases/


#### Where can I get help
If your answer is not found here the preferred method of support is via discord, but we also have a sub-reddit as well.  Please note that support via reddit may be delayed.

Rockin' The Classics Discord Server https://discord.gg/C9EDFyg  

/r/hakchi on Reddit https://reddit.com/r/hakchi/  

#### What systems does hakchi support?
NES classic edition  /  Famicom   
SNES classic edition  /  Super Famicon  
Sega genesis mini  /  Megadrive  

## Features
<details>
  <summary>hakchi 3.7.0 Features.</summary>


This release brings full UI integration to the Sega mini systems, it also makes use of additional space from the NAND that wasn't previously usable, so you get more space for all your games!

- New Features:
  - Bluetooth support with optional hmod available from the modules window
  - Sega Support!
    - Full stock UI integration
    - Folders
      - C button acts as a folder back button
    - Ability to force a specific UI theme
    - Support for launching Genesis/MegaDrive games in stock emulator
    - Support for launching games in other emulators
    - Save compression
    - Save compatibility with Retroarch and m2engage
    - Spine generator with templates by TheWez1981
    - Genesis/MegaDrive folder artwork by TheWez1981
  - Make use of additional space on the NAND that previously wasn't usable (applies to all hakchi systems)

To all the developers who have put in countless hours on this and previous builds, thank you!
</details>

***
## Supported devices
***
#### Bluetooth adapter  
ASUS USB-BT400  
https://www.amazon.com/dp/B00DJ83070  

TP-Link USB Bluetooth Adapter
https://www.amazon.com/dp/B07V1SZCY6?ref=ppx_pop_mob_ap_share

#### USB Wi-Fi adapter  
TP-Link USB Wi-Fi Adapter for PC N150  
https://www.amazon.com/dp/B008IFXQFU

Realtek Mini USB Wireless
802.11B/G/N LAN Card RTL8188
**Reported as working but only limited testing has been done**

#### Bluetooth controllers
- Switch pro controller
- PS4
- 8bitdo most SHOULD work
- 8bitdo M30
- 8bitdo SF30 pro

#### Wired controllers
- NES and SNES controllers will work on either system  
- USB controllers including PSC and Genesis/MegaDrive now work on SNES
- PSC controller will work on Sega post mod
- 8bitdo most should work in wired mode 
- Old Sega Saturn USB controller (cypress)  
- *Retrobit genesis 6 button and Saturn controllers both work (need mapping?)  
- Retro Fighters BrawlerGen Genesis Mini Controller 6 button

#### OTG adapters
https://www.amazon.com/gp/product/B07FY9Z9GD?pldnSite=1

https://www.amazon.com/gp/product/B00JCZ2FQQ?pldnSite=1

OTB hub
https://www.amazon.com/gp/product/B07XMBVQ2R?pldnSite=1

**Advanced - requires soldering**
MakerSpot Micro USB OTG Hub can be used if you feel up to soldering a USB end onto it.

**The small angled adapter is no longer recommended due to easily loses data connection at the slightest nudge.**



***
## hakchi
***
#### Menu items
#### Kernel
##### Install / Repair
Install or re-installs kernel mod and /hakchi (folder)
**This will update any existing hakchi scripts, but doesn't delete anything**

##### Reset
Reset  
:  Deletes /hakchi folder then installs it again
**This will delete any ROMs and HMODs from NAND**  
**Giving you a freshly flashed console**

##### Uninstall
Uninstalls /hakchi folder, ROMS, HMODs and kernel updates
**Completely removes hakchi mod and reverts they system back to stock**

*There is also a factory reset option that is like uninstall, but it also wipes your saves

#### Advanced
This section has advanced options you should only use when instructed by a dev.

#### Modules  
***
##### Install extra modules
Select which downloaded modules you want to install.  
If a module is greyed out it is already installed.

#### Uninstall extra modules
Select which installed modules you want to uninstall.

#### Generate modules report
Creates an HTML report with details of installed modules.

#### KMFD's Mod Hub
Hub / repository for downloading of RetroArch, cores and other options.

#### Manage mod repositories
Used for adding and removing repositories

#### View
***
Options for sorting the games list.

#### Settings
***
#### Language
Change the hakchi CE UI language

#### SEGA UI Theme
Allows the changing of the Sega UI  between United States, Europe and Japan

#### SFROM tool
TODO

#### Convert SNES ROMs to SFROM
TODO

#### Separate games storage
Creates separate a 'Games list' for each system in the UI.
These lists are maintained in separate folders in the hakchi2-ce folder.  
Examples:
- /games
- /games_md
- /mages_snes
etc...

#### Compress games when adding
TODO

#### Compress box art when adding
TODO

#### Center box art thumbnail
TODO

#### Disable hakchi2 popups
TODO

#### Separate games for multiboot
TODO

#### Always copy original games
TODO

#### Use linked sync
TODO

#### Global command line (Experts!)
TODO

#### Tools
***
##### Save state manager
TODO

#### Take screenshot
TODO

#### Save DMESG output

##### Open FTP client
Opens a file explorer window to transferring files to your mini

Shouldn't be needed when using this option, but if you need to enter the info manually:  
 
Host: 169.254.13.37
Port: 21
Login: root
Pass: none

*[FTP]: Host: 169.254.13.37 Port: 21 Login: root Pass: none

##### Open Telnet client
Remote telnet login to the system  

Host: 169.254.13.37
Port: 23
Login: root
Pass: none

#### Boot splash
TODO

#### Reboot
Sends reboot command to console

#### Switch running firmware
TODO

#### Format SD card
TODO

#### Prepare art folders
TODO

#### Bluetooth

#### Buttons and options
***

#### Games list
List of games currently added to hakchi.
Checked games are sync'd when selected.

Right clicking on games expands more options.
Select emulation core

#### Add more games
Adds more games to current games list

##### Export to USB
Syncs your checked games to a USB stick.  Requires  a USB 2.0 or 3.0 (system USB ports are only 2.0) formatted to EXT4 or NTFS.  
Insert USB into your PC running hakchi and press export.  
Safely remove  
While mini is powered off insert into port 2 or OTG on your mini. 
Power on  
 
When using USB storage on your mini and hakchi is connected the space estimation in the bottom right corner now reflects the USB storage.  And pressing SYNC now syncs with the USB NOT the mini.

##### Synchronize selected games with mini
Syncs all checked game from the game list to the mini when USB storage is not used.  If USB storage is used **AND** connected to the mini sync games will be sync'd to the USB  


#### Adding box art and spines
Single VS multiple



#### HMODs
TODO

***
## RetroArch
***
Ozone
XMB

#### Controller mapping
TODO

#### Install RetroArch
hakchi > Modules > KMFD's Mod Hub
KMDF RetroArch (tab)
Select your UI flavor
- Ozone (Grey list style)
- XMB (Playstation style)
Click 'Download and Install Module'

#### Install cores
hakchi > Modules > KMFD's Mod Hub
KMDF Cores (tab)
Either select individual cores and click 'Download and Install Modules'
OR 
Select various  modules and download them and use  
hakchi > Modules > Install extra modules

***
## General
***
#### When updating will I lose my saves
No

#### Can I launch RetroArch directly from the UI
Yes, install the "CLV-Z-RARCH" game and sync

#### I screwed up my mapping for my gamepad and can't reset it.
Reinstall RetroArch to get back to default settings

#### Enabling Wi-Fi
hakchi > Modules > KMFD's Mod Hub > KMFD System (tab) > WPA Supplicant  
Connect to the console using telnet/ssh
Type **wifi-wpa-setup** and enter your SSID and password when asked.  
Then follow instructions on screen  
USB Wi-Fi adapter can be plugged into any port on the Sega mini when instructed.  On S/NES it will be plugged into an OTG cable.
**While rebooting the Wi-Fi adapter must be the only USB device plugged in**
**Failure to do so will require un-installing WPA Supplicant and starting over**

#### Sega CD config
USB storage required due to the size of CD games
Pico core required when using multi-disk games
Genesis Plus GX required for CHD format games

Transfer bios files
With the console plugged to your PC and turned ON (green light in bottom left of hakchi CE):
-Tools > Open FTP client
-navigate to /etc/libretro/system
-upload your bios file(s) here

make sure they're correctly named, even the case is important! They MUST be:
-bios_CD_U.bin for US games
-bios_CD_E.bin for europe
-bios_CD_J.bin for japan



#### 32X 
Uses same bios as Sega CD, but only works with PicoDrive core


***
## SEGA
***
#### System details
OS - Linux
Controller ports - USB
Emulator - M2engage
ROM formats - 

Minimum power supply recommended  1.5

Additional storage space gained with hakchi CE 3.7    
Additional gained - 54mb
**Storage resize will revert back to stock after uninstalling**

Clock speed   
Stock - 1008000
Overclock - 1344000

##### Command line arguments:
 - --3bpad=1   
	Used for games like zombies ate my neighbors that won't work with 6 button pads  
	example - /bin/m2engage /var/games/CLV-G-XXSMB/Zombies_Ate_My_Neighbors.md.7z --3bpad=1  
 - --smooth43=1  
	command line for factory scan lines (stock emulator only)  
	
#### Overclock options
While overclocking your machine MAY become unstable and crash.  This is due to the quality of the manufactured CPU.  If you experience  crashing please disable any overclocking.

The **preferred method** of overclocking  is Easy Overclock.
Easy overclock from the Modules > KMFD's Mod hub > Games (tab).  When sync'd this "Game" is added to the UI menu to allow toggling  of overclock.  
	NOTE: Resets after power cycle  
	
Other but not preferred  methods.
Xtreme overclock is always active and can be found in Modules > KMFD's Mod hub > KMFD RetroArch (tab) > Xtreme Overclock
		NOTE: Can be verified  and toggled via telnet.  Stock freq - 1008000, Overclock freq - 1344000.
			 - hakchi overclock - Display current speed and temp
			 - hakchi overclock boot - Set default clock speed
			 - hakchi overclock max - Enables overclock

		NOTE: Maintains after power cycle
	
If --overclock is added to the command line of a RetroArch game the system will overclock for game then down clock on exit
 
	
 
#### Launching games from Sega UI  
  Press "A" to launch games with stock M2 emulator    
  Press "Start" to launch games with RetroArch (if installed)  
  To specify a core, Right click on a game from the hakchi "Custom Games" list and click "Select emulation core..."   
  
  When launching a game if a description does not exist it will launch directly into the game.  If a description does exist the standard game info box will pop up prior to game starting.
  
#### Installing after using other mods
  So hakchi detected modified files, what does this mean?  
	    
		"The system files appear to have been modified:
	    Version: MOON-mass-moon-es1-v0.8.3-108EU-1f2365d
	    Hash: dd5b58365b2104dfe89079a4c7c77ee4"  
	    Do you want to continue?

This means that a previous mod was detected on the system.  It is recommended that you completely uninstall the previous mod prior to continuing. 

***
## NES / SNES
***
#### System details  
OS - Linux  
Controller ports - Wii style  
Controller protocol = I²C

Clock speed   
Stock - 1008000
Overclock - 1344000


**NES
Storage size: 381.6MB, used: 17.0MB, free: 344.9MB
Storage size: 396.1MB, used: 17.6MB, free: 366.3MB

Additional storage space gained with hakchi CE 3.7
Storage size: 395.6MB, used: 19.5MB, free: 363.9MB
 
 
**Storage resize is permanent**

**SNES
Additional storage space gained with hakchi CE 3.7  
Pre mod -   
Additional gained - 
Post mod - 318mb
**Storage resize is permanent**

***
##  PlayStation classic
***
Currently there are no plans to support the PlayStation Classic.  
Other mods are available though.

Controller ports - USB

***
## Core and BIOS mapping
***
https://drive.google.com/file/d/1pd-_cy6fLKHvuWYD1s0e3cog3UKlq-B1/view
