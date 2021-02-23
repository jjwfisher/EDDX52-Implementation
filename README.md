# EDDX52 EDD Implementation

 A set of files for EDDiscovery, using the EDDX52 plugin dll files provided by EDDX52.
 
 - EDD (Elite Dangerous Discovery) is the tool used to create and program the Action files, which execute DLL calls based on in-game or external events.
 EDDcan be found here: https://github.com/EDDiscovery/EDDiscovery/
 
 - EDDX52 is a DLL made for interfacing EDDiscovery with the Saitek/Logitech x52 Pro joystick. This DLL and instructions for programming it can be found here: https://github.com/wulkanat/EDDX52/
 
 This repo is a collection of the files I have created using the two above tools, to program my joystick to respond to certain ingame events.
 #### This should work for any CMDR using these files, as the CMDR name/system info/ship info displayed on the MFD is information gained from EDD, via the game - so it does not need manually programming in. 
 #### All you need is: to know where to put these files (instructions given), and have a correctly set up (and up-to-date) installation of ED Discovery on your system.
 
 ## Please feel free to open a GitHub issue on this repo to request new features! 
 (in addition to reporting bugs, of course)
 
 ## This is currently very much a work in progress, and there are many bugs/broken features.
However, a summary of the current functionality is given below:
 
 #### For all of these features, anything written inside a pair of square brackets [], indicates that this is based on who is using the plugin. For example, on my system, "Welcome [CMDR Name]" will display as "Welcome CMDR EarthFishy"
 
 ### Boot:
 - Upon EDD boot, the LEDs will all turn off, and the MFD (LCD display on the throttle) will display: "Welcome, [CMDR Name]". After a 4 second pause, the MFD will display: "Waiting for ED Boot..."

- Upon loading the main game (into Solo, Private or Open play), the following is programmed:
 - LEDs: The LEDs will all simulaneously flash RED, AMBER, and GREEN colours, for 1 second each.
 - MFD: The MFD will initially display "Systems booting, please wait". After 1 second, it will display "Systems booting, loading..." whereby each dot is added after a 1 second pause, to give the impression of a loading screen (when in reality the MFD is being overwritten each time). Finally, roughly when the game has loaded (depending on how fast your game loads), the MFD will display "Welcome, [CMDR NAME]" in addition to "SHIP: [Ship Name], [Ship Ident]" which will be on the bottom line of the MFD. [Ship Ident] is the 3 letter/number long code you can give your ship in the Livery screen. 



## Disclaimer:
I hereby DO NOT accept any responsibility for any damage to hardware or software caused by these files, they are in an ALPHA state and use is entirely at your own risk.
