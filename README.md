# MDOS Utilities

Collection of Geneve 9640 Operating system utilities that I wrote and/or maintain.

From a build perspective, the utilities I publish here may have interdependencies across
various source folders. For example, PFM and CYA utilities rely on CRC common code.


## CRCOS7
Operating system CRC verification utility. CRCMAINS is used by other utilities.
The CRC installer utility is only distributed to MDOS developers.

## PFM
Utilities to support the PFM512 and PFM+ onboard flash hardware. 
512K -  Atmel 29c040/29c040a and Winbond 29c040 512KiB 
285K -  Atmel 29c020 * 2 (256KiB) version

## TSTAT
TIPI utility. Detects updates to the TIPI (RPi side) and allows the user 
to update, halt, restart, and display the EPROM version string. 

## BBRM
Backup Bit Remover utility.  Strips the "Backup" archive bit from a file's descriptor record. 
In the 90s, the problem was most noticeable with MENU and its variants for the Horizon Ramdisk. 
Affected files will show up as unknown file types in these programs.  The Horizon ROS was updated
to resolve this issue at the DSR level however, old disks/files may benefit from this fix. 

## CFG
GenCFG formatter/utility for the Horizon Ramdisk.   Also see
https://github.com/horizonramdisk/Horizon-Ramdisk-ti994a/wiki

