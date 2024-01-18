# Tips/Tricks for Upgrading a Drive
Upgrading your computer's drive from a HDD to a SSD, or a smaller drive to a bigger drive, can be a bit overwhelming. 

Hopefully this guide will help you to success.

## WARNING
DO THIS AT YOUR OWN RISK. I OFFER NO WARRENTY FOR ANY DAMAGE DONE TO YOUR DISK. CONTINUING TO READ THIS DOCUMENT IS VALID AS AN AGREEMENT TO NO WARRENTY.

IF USING A BATTERY POWERED DEVICE, PLUG IN THE DEVICE AT ALL TIME. THE DEVICE POWERING OFF CAN CAUSE PERMEMANT DATA LOSS.

USE AT YOUR OWN RISK. IT IS HIGHLY RECCOMENDED TO DO A FILE-BASED BACKUP FIRST.

## Options

## Size
- 3.5
- 2.5
- M.2

## Hardware
- SATA to USB
- External SATA Enclosure
- CD/DVD Drive to HDD/SSD Drive

## File Based vs Block Based 
- Windows
  - robocopy
  - xcopy
  - copy
- macOS/Linux
  - rsync
  - cp

## Cloning a Disk

Do not use [dd](https://en.wikipedia.org/wiki/Dd_(Unix)).

Use a live linux iso on an external drive. When you clone a disk, you need to make sure that no files are being edited/copied in the background. Using Clonezilla/Rescuezilla gurantee no files are being edited in the background.

- [Clonezilla](https://clonezilla.org/)
- [Rescuezila](https://rescuezilla.com/)

ISSUES TO LOOK OUT FOR: 
- IF USING WINDOWS
  - Use this shutdown command to fully shut the system down: ```shutdown /s /f /t 0```
  - Windows does not allow you to boot a cloned system drive from USB.
  - ```diskmgmt```

BIOS
- Check device manual for bios/boot button.
- Check CSM is enabled
- Secure Boot is disabled before using clonezilla/rescurezilla.
- Disable Fast Boot if not able to access boot menu easily
- Check Hard Drive BBS Priorties if Clonezilla/Rescurezilla drive does not appear.

CLONE TO DISK OR CLONE TO IMAGE

AFTER CLONE
- If moving upgrading from HDD to SSD
  - To use the HDD as a secondary drive, you will need to reformat it.
    - It needs to be changed from a C:\ drive to another letter.  

Videos:
- [What are Drive Imaging and Drive Cloning?](https://www.youtube.com/embed/jrJTQF3o5c4)
- [EASY WAY TO Migrate Windows to Another Drive, FOR FREE! Boot Media with Rescuezilla](https://www.youtube.com/embed/znQXKbJvdtY?t=67)
- [Clone Any System (using Clonezilla)](https://www.youtube.com/embed/yQ9NpWZ74BU?t=66)
- [Drive Cloning & Imaging](https://www.youtube.com/embed/UTsq-HHz0Ss) //Uses Macrium
- [Free Drive Cloning Applications](https://www.youtube.com/embed/1gTJw8ehkVc)

The most common pitfall is trying to clone a LARGER drive into a SMALLER drive. This can be done with [gparted](https://en.wikipedia.org/wiki/GParted).

## RAID (Reduency, not a Backup)
- RAID1 (Mirroring)

## RAID VIDEOS
- [RAID 0, RAID 1, RAID 10 - All You Need to Know as Fast As Possible](https://www.youtube.com/embed/eE7Bfw9lFfs)
- [What is RAID 0, 1, 5, & 10?](https://www.youtube.com/embed/U-OCdTeZLac)
- [Set up RAID 1 Mirroring on Window 10 Pro](https://www.youtube.com/embed/7nga6Nydy3M)
- [Hardware Raid is Dead and is a Bad Idea in 2022](https://www.youtube.com/embed/l55GfAwa8RI)

## Backup
- External Drive/Card
- NAS
- Cloud
