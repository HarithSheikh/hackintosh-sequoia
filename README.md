# Hackintosh EFIs for Gigabyte B760M, Intel Core i5 14600K, AMD Radeon RX 6600



# Basic Information

**EFIs**: macOS Sequoia Latest
<br>
**Current OpenCore**: 0.8.8
<br>
**Release date**: 18/08/26

# Hackintosh Specifications
|Item|Description|
|-|:-------:|
|Motherboard|Gigabyte B760M DS3H DDR4|
|CPU|Intel Core i5 14600K|
|Memory|2x 16Gb DDR5 Cosair Vengence 3200Mhz|
|dGPU|AMD Radeon RX 6600|
|Ethernet|Realtek Gaming 2.5GbE Family Controller|
|Wireless/BT|Fenvi/Broadcom BCM94360 4 Antenas|
|Storage|KINGSTON 1TB |

## EFI Creator
- [Harith Sheikh](https://github.com/harithsheikh)
- This was made following many trial and error and a preset.

## SMBIOS (Important)
- Din't pay much attention to this but matters a lot as some models get more performance over other and you must not use a real mac or reuse details.
- iMacPro1,1 gave me best performance up till now.

## Folder Contain
- 2x EFI

## EFI Choose
- use my EFI v1 as it is more optimised and simple. If it doesn't work then use EFI 2.
- If my EFI dont help, try OpCoreSimplify. Dint help me but might be useful for you.

## Motherboard Settings
- Basic changes, CSM Disabled, 4G Decoding enabled, VT-D off if you dual boot. IGPU preferably off.
  
## Setup Guide (Windows)
- use mcrecovery tool from OpenCore to generate your recovery file
- Download one of my EFI
- Use a tool like ProperTree or OCAT to edit/generete a new SMBIOS (Serial Number, ect.)
- Modify the file if you know what you are doing.
- Put those both the folders into a usb formatted with preferable Rufus.. 

## Setup Guide (MacOS/existing hackintosh)
- If you already have macos/hackintosh, install the desired macOS through recommended App Store or terminal.
- Make a bootable usb along with it (Format and copy files auto)
- Use OCAT to mount the efi folder and copy your modified efi folder into it.

## BCM94360 WiFi / Bluetooth
- Up till ventura it's supported natively and wont need extra kexts however in this MacOS version you will need to use OCLP which might require lowering SIP and bypassing AMFI which could reduce your security.

## Feedback
- Haven't experienced any major issues after initial setup and tweaking period. works smooth. Sometimes rarely might get a 0.5 second freeze but goes away. SMBIOS Model matters a lot for performance, best way to check the best model for you is geekbench check windows and then on macos. Closest result i got was with iMacPro1,1. I decided not to go with OCLP right now as I want security so my wifi andf bluetooth arent functional and features like airdrop, continuity and screen mirroring doesn't work. AppleID, passkeys other sync, apps work perfectly.
- Fun fact, I was using this EFI for Tahoe before.

## Issues I ran during initial.
1. Glitched Screen or booting errors.
- Fix by using display port on RX6600 or iGPU for setup only.
2. Stuck in Bootloop
- Mess with the boot arguments as thats what helped me.
3. After Setup, services not working.
- use a invalid SMBIOS.
4. More Problems
- Try other EFI or contact.


## Contact
- I can be reached out through discord at @hsheikh24 (preferable) or email at contact@bloxtuan.com
