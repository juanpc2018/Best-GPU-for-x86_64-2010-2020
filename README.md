### Best GPU for x86_64 (2010-2020) </br>

### The title of this Repo is "Best GPU for.."
The goal is to find 1x GPU that works in all OS, or most. </br>

most important OS from x86_64 era: </br>
[OSX SnowLeopard 10.6.8](https://en.wikipedia.org/wiki/Mac_OS_X_Snow_Leopard) </br>
[OSX Mavericks 10.9.5](https://en.wikipedia.org/wiki/OS_X_Mavericks) </br>
[OSX HighSierra 10.13.6](https://en.wikipedia.org/wiki/MacOS_High_Sierra)  </br>
[OSX Mojave 10.14.x](https://en.wikipedia.org/wiki/MacOS_Mojave) </br>
[OSX Catalina 10.15.7](https://en.wikipedia.org/wiki/MacOS_Catalina) </br>
[Windows 8.1 (2013-2023)](https://en.wikipedia.org/wiki/Windows_8.1) </br>
Ubuntu / Kubuntu 10.04 LTS to *buntu 22.04.4 LTS x86_64 or similar .deb </br>

for many Reasons: </br>
OSX SnowLeopard 10.6.8 has [Rosetta](https://en.wikipedia.org/wiki/Rosetta_(software)) PowerPC G4 "emulator" Binary Translation, removed / deleted in OSX Lion 10.7 </br>
OSX Mavericks 10.9.5 is the last OS that works with ProTools HD10.3.10 also has 3rd party USB3.0 drivers for VL800 chip, and old Renesas Firmware, Not compatible in following OSX </br>
OSX HighSierra 10.13.6 is the peak of 32-Bit & 64-Bit , .3 has Thunderbolt2 eGPU support, .4 removed TB2 eGPU support and added TB3 eGPU support, requires a patch to reactivate TB2 eGPU in .6 </br>
HighSierra also Read/Writes & Formatts APFS drives. </br>
OSX Mojave 10.14 removes 32-Bit driver support, the last to support QuickTime required for ProTools & Avid Media composer Video Engine. </br> 
OSX Catalina 10.15.7 is the last 100% intel, 100% 64-Bit, removed 32-Bit completely, preparing for the transition to ARM M CPU's </br>
OSX BigSur 11, using a RAM drive of 2GB, and a test file of 1GB in [Black Magic Speed Test](https://apps.apple.com/us/app/blackmagic-disk-speed-test/id425264550?mt=12) or [AJA Speed Test](https://www.aja.com/products/aja-system-test), The Hybrid Kernel Runs slower on x86_64 vs. OSX Catalina pure x86_64 kernel. </br>
BigSur 11 takes too much time to update from OSX Catalina, and does Not allow to Downgrade. </br>

OSX SnowLeopard 10.6.8 cannot be installed on a Mac newer than 2010, </br>
unless using a Virtual Machine like VMWare Fusion Player 10.2.1 on OSX Catalina </br>
but VM does Not have FireWire support, Nor Firewire Pass-through, Nor PCIe Pass-through. </br>
OSX SnowLeopard is designed for MacPro 5,1 2010 with AMD Radeon HD 5770, HD 5870, HD 7950, GTX Titan 6GB, K5000, Quadro 4000, and others. </br>

Running a more recent VMWare than >10.2.1 requires OSX BigSur or Newer, but OSX Hybrid Kernel becomes -30% slower. </br>

Windows 8.1 is similar to OSX HighSierra, the Peak of 32-Bit & 64-Bit. </br>
but Steem, Origin, Ubisoft re-compliled Launchers so it does Not work on Windows8.1 anymore = Gaming on Win8.1x64 is dead, unless its retro gaming, but some games like Need For Speed The Run probably wont work, </br>
because requires Origin app account, Discontinued and Replaced by EA app. </br>
but still Win8.1 is important for other Windows Only software like [Microchip Studio for AVR & SAM Devices 7.0.2594 (20 Jun 2022)](https://www.microchip.com/en-us/tools-resources/develop/microchip-studio) and older,
for programmers like [STK 600](https://www.microchip.com/en-us/development-tool/ATSTK600) and older STK500, etc..., that require USB drivers. </br>
but if Only requires USB drivers, probably is better to install Win8.1x64 in a Virtual Machine with USB pass-through. </br>

## GPU candidates:

AMD latest driver that supports Win8.1 officially was for RX 480, forcing W7 driver for Rx 580 may work, but untested, Not official. </br>
basically AMD is discarded for Win8.1x64. </br>
Nvidia latest GPU that has drivers for Win8.1 is RTX 8000, P6000, Titan Xp, M6000 </br>
but... RTX 8000 does Not work in OSX Mavericks 10.9.5 requires to buy 2x GPUs or another GPU more compatible with different OS </br>

Windows 8.1 works in [ASRock Z790 LiveMixer](https://www.asrock.com/mb/Intel/Z790%20LiveMixer/Specification.asp) UEFI v9.03 + [ASRock Thunderbolt 4 v1](https://www.asrock.com/mb/spec/product.asp?Model=Thunderbolt%204%20AIC)
using Dual Boot: Linux & Win8.1 on separate SSD or M.2 </br>
requires a GPU compatible with Windows8.1 </br>
having a powerful GPU for Windows is pointless because Modern 3D Gaming is Dead in Win8.1 unless its DRM Free like GOG </br>
is better to game in Linux using Wine, Codeweavers, Bottles, Proton, PlayOnLinux </br>
but Not everything works in Linux, </br>
for example: </br>
ProTools Ultimate 2020.12 + HDX PCIe </br>
ProTools HD10.3.10 + HD PCI-x or PCI-e </br>
ilok VST2 plugins work in Linux IF plugin allows to store license on the Machine, Not USB, because ilok-USB requires propietary drivers Not available for Linux. </br>
Matrox MXO2 MAX + Adobe CS6 Media Encoder / Avid Video Engine </br>
imacon Photo / 343 / 646 / 848 / 949 SCSI A-sync scanner with FlexColor v4.0 software </br>
and others... </br>

Best GPU for Dual Boot: </br>
Low Cost: GT 1050 Ti, the perfect option, has DisplayPort for New Monitors like LG 34GP63A that require DP to run at 160fps, and Low power consumption. </br>
Fastest GPU: RTX 8000, P6000, Titan Xp, M6000, IF want Dual Boot Win8.1x64 + Linux to Game on Linux, but in Windows a fast GPU will be overkill, very few software will use it. </br>
using a Modern / Faster GPU like 4070 or 4070 Super "The best in the 200w category" works on Linux but Not on Win8.1 </br>
requires to turn-off & open the PC, change GPU's and boot in other OS, or install 2x different GPU's at same time, or purchase a Twin machine to have different GPU's & different OS. </br>

OSX Mavericks 10.9.5 works with GTX Titan 6GB / GTX 780 "the same" and M6000 "+50% faster" </br>
GTX Titan 6GB / GTX 780 are the true sucessor of Nvidia GTX 580 </br> 
GTX 680 series were a dissapointment in my opinion, a cut down version with higher clock to compensate, did Not feel an improvement on games like NFS The Run. </br>
but GTX 680 can be flahsed easy to have EFI and Boot on MAC OSX, same as Radeon HD 7950 </br>

P5000 is +20% faster vs. M6000 but slower vs. Titan X "Maxwell" and much slower vs. Titan X "pascal", and much slower vs. Titan Xp </br>
But the fastest Titan Xp, is very slow vs. RTX 3070 or better. </br>
using a GPU compatible with Win8.1 & Linux will Not allow to play modern RayTracing Games like Indiana Jones - The Great Circle (2024) unless its a RTX 8000 </br>
but RTX 8000 wont work in OSX if you also have a Mac Pro 5,1 2010 or a MacPro 6,1 2013 or MacMini 2014 with TB2 eGPU </br> 
