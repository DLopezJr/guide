# Tips/Tricks for Upgrading a Drive
Upgrading your computer's drive from a HDD to a SSD, or a smaller drive to a bigger drive, can be a bit overwhelming. 

Hopefully this guide will help you to success.

## WARNING
DO THIS AT YOUR OWN RISK. I OFFER NO WARRENTY FOR ANY DAMAGE DONE TO YOUR DISK. CONTINUING TO READ THIS DOCUMENT IS VALID AS AN AGREEMENT TO NO WARRENTY.

IF USING A BATTERY POWERED DEVICE, PLUG IN THE DEVICE AT ALL TIME. THE DEVICE POWERING OFF CAN CAUSE PERMEMANT DATA LOSS.

USE AT YOUR OWN RISK.

## Options

## Size
- 3.5
- 2.5
- M.2

## Hardware
SATA to USB
External SATA Enclosure
CD/DVD Drive to HDD/SSD Drive

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

Rescuezilla is easier for most people, but Clonezilla has been around forever.

- [Clonezilla](https://clonezilla.org/)
- [Rescuezila](https://rescuezilla.com/)

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
